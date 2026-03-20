# P123 AI Factor API Reference

## Table of Contents
1. [Overview](#overview)
2. [aifactor_predict() — Get AI Factor Predictions](#predict)
3. [Parameters](#parameters)
4. [Response Schema](#response)
5. [DataFrame Output](#dataframe)
6. [Quota & Credits](#quota)
7. [Using Predictions in Formulas](#formulas)
8. [Common Patterns](#patterns)
9. [Operational Gotchas](#gotchas)

---

## Overview <a name="overview"></a>

P123's AI Factor system trains machine learning models (typically LightGBM) on user-defined feature sets to predict future stock returns. The API provides a single prediction endpoint — training, feature configuration, and model management are done through the P123 web UI only.

**Key concepts:**
- **AI Factor**: A saved configuration containing features, universe, training parameters, and one or more predictors
- **Predictor**: A trained model within an AI Factor (e.g., "LightGBM" or "XGBoost"). Each has a unique numeric ID
- **Prediction**: The model's output score for each stock in the universe (higher = expected better return)
- **Features**: The input variables fed to the model (P123 formulas). The API can return both feature names and their transformed values

**What the API can do:**
- Retrieve current predictions for all stocks in a predictor's universe
- Retrieve historical predictions as of any past Saturday
- Include feature names and transformed feature values
- Include company names and FIGI identifiers

**What the API cannot do (UI only):**
- Create, edit, or delete AI Factors
- Configure features, universes, or training parameters
- Trigger training runs
- View model performance metrics (IC, Sharpe, feature importance)
- List available AI Factors or predictors

---

## aifactor_predict() — Get AI Factor Predictions <a name="predict"></a>

```python
client.aifactor_predict(predictor_id, params={}, to_pandas=False)
```

Returns predictions for all stocks in the predictor's trained universe.

### Basic Usage

```python
import p123api

client = p123api.Client(api_id='YOUR_ID', api_key='YOUR_KEY')

# Get current predictions (returns dict)
result = client.aifactor_predict(123456)

# Get as DataFrame
df = client.aifactor_predict(123456, {}, to_pandas=True)
```

### With All Options

```python
result = client.aifactor_predict(
    predictor_id=123456,
    params={
        'asOfDt': '2026-03-14',        # Historical predictions (must be Saturday)
        'includeNames': True,           # Add company names
        'includeFeatures': True,        # Add feature names + transformed data
        'figi': 'Country Composite',    # Add FIGI identifiers
        'pitMethod': 'Complete',        # Point-in-time method
        'precision': 4,                 # Decimal places (2–6)
    },
    to_pandas=True
)
```

---

## Parameters <a name="parameters"></a>

The `p123api` wrapper passes all `params` through to the server unchanged — it performs no client-side validation. The accepted/rejected parameters below were determined by testing against the live API (March 2026, p123api v2.2.0). Server-side behavior may change.

| Parameter | Type | Required | Default | Description |
|-----------|------|----------|---------|-------------|
| `predictor_id` | int | **Yes** | — | Numeric ID of the trained predictor. Found in P123 UI under AI Factor settings. This is a positional argument, not part of `params`. |
| `asOfDt` | string | No | current | Historical prediction date. **Must be a Saturday** (e.g., `'2026-03-14'`). Returns predictions as they were on that date. |
| `includeNames` | bool | No | False | Include company names in response (`names` field). |
| `includeFeatures` | bool | No | False | Include feature names (`features` field) and transformed feature matrix (`data` field). |
| `figi` | string | No | — | Include FIGI identifiers. Values: `'Country Composite'` or `'Share Class'`. |
| `pitMethod` | string | No | See note | Point-in-time method. `'Complete'` waits for all data; `'Prelim'` uses preliminary filings. As of March 2026, the API default appears to be `'Prelim'` (predictions match explicit Prelim when aligned by p123Uid), though P123 has changed the frontend default to Complete. Recommend always setting this explicitly. |
| `precision` | int | No | 2 | Decimal precision for predictions. Accepted values: `2`, `3`, `4`, `5`, or `6`. Values outside this range (0, 1, 7+) are rejected. |

### Parameters Not Accepted (Observed)

These parameters work on other P123 API endpoints but are **rejected by the server** when passed to AI Factor predict (returns `"Unrecognized parameter"` error):

| Parameter | Use Instead |
|-----------|------------|
| `tickers` | Cannot filter — always returns full universe |
| `currency` | Predictions are unitless scores, not currency-denominated |
| `region` | Universe is fixed at training time |
| `type` | Stock/ETF type is fixed at training time |
| `rankingMethod` | Not applicable — predictions are raw model outputs |
| `includeRawData` | Raw (untransformed) data may be returned server-side based on AI Factor config, but cannot be requested via params |

---

## Response Schema <a name="response"></a>

The response schemas below were observed from live API calls (March 2026). The wrapper only accesses `p123Uids`, `tickers`, `predictions`, `names`, `figi`, `features`, `data`, and `rawData` — other fields like `cost`, `quotaRemaining`, `priceDt`, `updateDt`, and `dt` are passed through but not used by the wrapper.

### Current Predictions (no `asOfDt`)

```json
{
    "cost": 20,
    "quotaRemaining": 5247,
    "priceDt": "2026-03-19",
    "updateDt": "2026-03-20T04:03:19.94-05:00",
    "p123Uids": [101646, 104770, ...],
    "tickers": ["BERNER.B:SWE", "TTR1:DEU", ...],
    "predictions": [0.24, 0.27, ...]
}
```

### Historical Predictions (with `asOfDt`)

```json
{
    "cost": 20,
    "quotaRemaining": 4947,
    "dt": "2026-03-14",
    "p123Uids": [101646, 104770, ...],
    "tickers": ["BERNER.B:SWE", "TTR1:DEU", ...],
    "predictions": [0.29, 0.27, ...]
}
```

The response schema changes between current and historical calls:
- **Current**: Returns `priceDt` (last price date) + `updateDt` (model update timestamp)
- **Historical**: Returns `dt` (the requested Saturday) only — no `priceDt` or `updateDt`

### With Optional Fields

When `includeNames=True`:
```json
{
    "names": ["Berner Kantonalbank AG", "technotrans SE", ...]
}
```

When `includeFeatures=True`:
```json
{
    "features": [
        "Revenue Recognition Quality (Skip + Date & Sector)",
        "Distance from SMA (Skip + Skip)",
        ...
    ],
    "data": [
        [2.66, 95.0, -0.492, ...],
        [-0.471, 45.0, 1.39, ...],
        ...
    ]
}
```

- `features`: List of feature names (length = number of features in the model)
- `data`: 2D array (stocks × features) of **transformed** feature values (after P123's preprocessing/normalization)

When `figi='Country Composite'` or `figi='Share Class'`:
```json
{
    "figi": ["BBG005NR9YT8", "BBG005C4M635", ...]
}
```

### Raw Data

Some AI Factor configurations return a `rawData` field alongside `data`. This contains the **untransformed** feature values. This is controlled by the AI Factor's server-side configuration — it cannot be toggled via API parameters. When present:

```json
{
    "rawData": [
        [1.23, 45.6, -0.78, ...],
        ...
    ]
}
```

The DataFrame output (with `to_pandas=True`) automatically prefixes raw columns with `"raw "` (e.g., `"raw Revenue Recognition Quality (Skip + Date & Sector)"`).

---

## DataFrame Output <a name="dataframe"></a>

With `to_pandas=True`, the response is converted to a DataFrame:

### Minimal (no optional params)

```
   p123Uid       ticker  prediction
0    87864      WAF:DEU       -0.08
1    86053    1CNHI:ITA        0.07
2    82135    KENDR:NLD        0.10
```

### With `includeNames=True`

```
   p123Uid       ticker                          name  prediction
0    87864      WAF:DEU                  Siltronic AG       -0.08
1    86053    1CNHI:ITA           CNH Industrial NV        0.07
```

### With `includeFeatures=True`

```
   p123Uid  ticker  prediction  Revenue Recognition Quality (Skip + Date & Sector)  Distance from SMA ...
0    87864 WAF:DEU       -0.08                                               2.66                           95.0 ...
```

Shape: (num_stocks, 3 + num_features). With 500 features: `(1038, 503)`.

If `rawData` is present, raw columns are appended with `"raw "` prefix, doubling the feature columns.

---

## Quota & Credits <a name="quota"></a>

| Metric | Value |
|--------|-------|
| Cost per call | **20 credits** (fixed, regardless of params or universe size) |
| Monthly quota | Varies by subscription tier (check `quotaRemaining` in any response) |

The `quotaRemaining` field in every response shows your remaining credits for the current billing period.

**Quota management tips:**
- Cache predictions — they update once daily (check `updateDt`)
- Use `asOfDt` sparingly for backtesting — each historical call costs the same 20 credits
- Reserve capacity for rebalancing periods when you need fresh predictions
- `includeFeatures` does NOT cost extra credits (same 20 per call)
- The quota is shared across all API operations — see the API Credits & Limits section in `api-reference.md`

---

## Using Predictions in Formulas <a name="formulas"></a>

AI Factor predictions can be used directly in P123 screens and ranking systems:

```
// Reference a prediction in a screen rule
AIFactor("My AI Factor", "lightgbm predictor") > 0

// Rank by AI prediction
FRank(`AIFactor("My AI Factor", "lightgbm predictor")`, #All, #DESC) > 80

// Validation mode (uses walk-forward OOS predictions)
AIFactorValidation("My AI Factor", "Model Name")

// With duplicate ID for multiple models on same factor
AIFactorValidation("My AI Factor", "Model Name", "dup_id")
```

**Note:** `AIFactor()` uses the latest trained prediction. `AIFactorValidation()` uses the walk-forward out-of-sample predictions — this is what you should use for backtesting to avoid look-ahead bias.

---

## Common Patterns <a name="patterns"></a>

### Download Predictions for Portfolio Construction

```python
# Get predictions with company names for review
df = client.aifactor_predict(123456, {
    'includeNames': True,
    'precision': 4
}, to_pandas=True)

# Sort by prediction (highest = best expected return)
df_sorted = df.sort_values('prediction', ascending=False)

# Top 50 picks
top_picks = df_sorted.head(50)
print(top_picks[['ticker', 'name', 'prediction']].to_string())
```

### Compare Current vs Historical Predictions

```python
# Current predictions
current = client.aifactor_predict(123456, {}, to_pandas=True)

# Last week's predictions (Saturday date)
historical = client.aifactor_predict(123456, {
    'asOfDt': '2026-03-14'
}, to_pandas=True)

# Merge and compare (inner join — drops stocks not in both dates)
merged = current.merge(historical, on='p123Uid', suffixes=('_now', '_prev'))
merged['delta'] = merged['prediction_now'] - merged['prediction_prev']
big_movers = merged[merged['delta'].abs() > 0.1].sort_values('delta', ascending=False)
```

### Extract Feature Data for Local ML Training

```python
# Get all features for local analysis
df = client.aifactor_predict(123456, {
    'includeFeatures': True,
    'includeNames': True,
    'precision': 4
}, to_pandas=True)

# Separate predictions from features
meta_cols = ['p123Uid', 'ticker', 'name', 'prediction']
feature_cols = [c for c in df.columns if c not in meta_cols]

X = df[feature_cols]
y = df['prediction']

# Feature importance via correlation with prediction
correlations = X.corrwith(y).abs().sort_values(ascending=False)
print("Top 10 features by correlation with prediction:")
print(correlations.head(10))
```

### Upload Custom Predictions as Stock Factor

```python
# Get AI Factor predictions
df = client.aifactor_predict(123456, {}, to_pandas=True)

# Create CSV for stock factor upload (date, ticker, value)
import datetime
today = datetime.date.today().strftime('%Y-%m-%d')
upload_df = df[['ticker', 'prediction']].copy()
upload_df.insert(0, 'date', today)
upload_df.to_csv('/tmp/ai_predictions.csv', index=False, header=False)

# Upload as custom stock factor
client.stock_factor_upload(
    factor_id=YOUR_FACTOR_ID,
    data=open('/tmp/ai_predictions.csv'),
    column_separator='comma',
    existing_data='overwrite',
    date_format='yyyy-mm-dd'
)
```

---

## Operational Gotchas <a name="gotchas"></a>

### One Request at a Time Per API Key

The P123 API enforces a single concurrent request per API key. If you send a second request while the first is still processing, the server returns:

```
API request failed: You already have an API request in progress
```

This means you cannot parallelize API calls. When scripting multiple predictions (e.g., comparing predictors or historical dates), add a short delay between calls or wait for each response before sending the next.

### Saturday Dates Are Mandatory for Historical Calls

```python
# ❌ Wrong — any non-Saturday raises an error
client.aifactor_predict(123456, {'asOfDt': '2026-03-16'})
# "asOfDt must be a Saturday if specified"

# ✅ Correct — use Saturday dates
client.aifactor_predict(123456, {'asOfDt': '2026-03-14'})
```

This differs from `data_universe()` which accepts arbitrary dates (any day of the week), though its underlying data appears to use a weekly snapshot that changes on Saturdays. AI Factor is stricter — it requires Saturday specifically.

### Response Schema Differs Between Current and Historical

```python
# Current call returns priceDt + updateDt
result = client.aifactor_predict(123456)
result['priceDt']   # "2026-03-19"
result['updateDt']  # "2026-03-20T04:03:19.94-05:00"

# Historical call returns dt (no priceDt or updateDt)
result = client.aifactor_predict(123456, {'asOfDt': '2026-03-14'})
result['dt']        # "2026-03-14"
result['priceDt']   # ❌ KeyError — field doesn't exist in historical response
```

### Universe Size May Vary Between Dates

Current predictions may return a different number of stocks than historical predictions (e.g., 1,038 current vs 1,024 historical). This reflects changes in the underlying universe over time — stocks being added/removed, delisted, etc.

### Predictions Are Unitless Scores, Not Returns

The `prediction` values are model output scores, not expected return percentages. Their scale depends on the model's training target and normalization. Use `FRank()` in P123 formulas to convert to percentile ranks for ranking and screening.

### Predictions Can Be Null

Not every stock receives a prediction. In practice, ~3–4% of the universe may have `None`/null predictions (observed on live calls). This can happen when a stock lacks sufficient data for the model to score. Always handle nulls when sorting, uploading to stock factors, or feeding predictions into downstream analysis:

```python
df = client.aifactor_predict(123456, {}, to_pandas=True)
df = df.dropna(subset=['prediction'])  # Remove null predictions
```

### No Ticker Filtering

Unlike `data_universe()` or `rank_ranks()`, you cannot request predictions for specific tickers. Each call returns the **entire universe**. Filter client-side:

```python
df = client.aifactor_predict(123456, {'includeNames': True}, to_pandas=True)
my_stocks = df[df['ticker'].isin(['AAPL', 'MSFT', 'GOOG'])]
```

### Feature Names Include Transformation Info

Feature names follow the pattern: `"Feature Name (Transform1 + Transform2)"`. The parenthetical describes P123's preprocessing:
- `Skip` = no transform applied at that stage
- `Date` = date-normalized (cross-sectional within each date)
- `Sector` = sector-normalized
- `Date & Sector` = both date and sector normalized

### Training and Config Are UI-Only

The API provides **no endpoints** for:
- Listing your AI Factors or their predictor IDs
- Reading feature lists or model configuration
- Triggering training runs
- Viewing IC, Sharpe, or other model metrics

You must find predictor IDs through the P123 web interface. Keep a local record of your predictor IDs and what they contain.

### API Quota Is Shared

The monthly credit quota is shared across **all** API operations (data retrieval, screening, backtesting, AND AI Factor predictions). Heavy API backtesting can exhaust quota needed for AI Factor prediction calls. Budget accordingly.
