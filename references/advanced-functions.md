# P123 Advanced Functions Reference

## Table of Contents
1. [SetVar / ShowVar — Variables](#setvar)
2. [Eval & NA/Neg Replacement — Conditional Logic](#eval)
3. [FRank — Cross-Sectional Percentile Rank](#frank)
4. [ZScore — Cross-Sectional Z-Score](#zscore)
5. [FOrder, FCount, FSum, FMedian — Cross-Sectional Utilities](#forder)
6. [Aggregate — Cross-Sectional Statistics](#aggregate)
7. [Scope Parameter Values](#scope)
8. [FHist — Historical Time Series](#fhist)
9. [FHistRank, FHistRel, FHistZScore — Relative vs History](#fhistrank)
10. [Loop Functions — Iteration with CTR](#loop)
11. [Regression Functions & Statistics](#regression)
12. [NodeRank & Ranking Functions](#noderank)
13. [AI Factor Functions](#aifactor)
14. [Screen-Only Functions](#screen-only)
15. [Universe Operations (Strategy)](#universe-ops)
16. [Consensus Estimate Functions](#consensus)
17. [Surprise Functions](#surprises)
18. [Dividend & Corporate Action Functions](#dividends)
19. [Insider Functions](#insider)
20. [Institutional Functions](#institutional)
21. [Short Interest](#shortinterest)

---

## SetVar / ShowVar — Variables <a name="setvar"></a>

```
SetVar(@name, expression)
```

- Variable names start with `@`
- Evaluated once, cached for the stock being processed
- Chain multiple SetVars; use in subsequent expressions

**Display in report** (two ways):
```
@name:expression              // colon syntax — sets, displays, and returns value
ShowVar(@name, expression)    // ShowVar — sets variable and displays in report
```

```
SetVar(@pe, PEExclXorTTM)
SetVar(@cheap, @pe < 15)
SetVar(@quality, ROE%TTM > 15 AND GMgn%TTM > 40)
@cheap AND @quality

// ShowVar for grouping in screen reports
ShowVar(@group, Eval(DivYield%TTM=0, 0, Eval(DivYield%TTM > 5, 2, 1)))
ShowVar(@groupAvgCap, Aggregate("MktCap", #GroupVar, #Avg))
MktCap < @groupAvgCap
```

---

## Eval & NA/Neg Replacement — Conditional Logic <a name="eval"></a>

### Eval

```
Eval(condition, true_value, false_value)
```

```
// Use alternate metric when PE is NA
Eval(IsNA(PEExclXorTTM), Pr2SalesTTM, PEExclXorTTM)

// Sector-specific logic
Eval(SectorId = 40, DbtTot2EqQ < 15, DbtTot2EqQ < 2)

// Nested multi-branch
Eval(MktCap > 10000, 1, Eval(MktCap > 2000, 2, Eval(MktCap > 300, 3, 4)))

// Winsorize
Eval(PEExclXorTTM > 100, 100, Eval(PEExclXorTTM < 0, 0, PEExclXorTTM))
```

### Replacement Functions

| Function | Description |
|----------|-------------|
| `IsNA(expr1, expr2)` | Returns `expr1` if not NA, otherwise `expr2` |
| `IsNeg(expr1, expr2)` | Returns `expr1` if not negative, otherwise `expr2` |
| `IsNegOrNA(expr1, expr2)` | Returns `expr1` if not negative and not NA, otherwise `expr2` |
| `IsZero(expr1, expr2)` | Returns `expr1` if not zero, otherwise `expr2` |

```
// Replace NA PE with 999
IsNA(PEExclXorTTM, 999)

// Replace negative FCF with 0
IsNeg(FCFTTM, 0)
```

---

## FRank — Cross-Sectional Percentile Rank <a name="frank"></a>

```
FRank("formula" [, scope=#All, sort=#DESC, incl_na=#InclNA, sort_style=#Top])
```

**Returns**: 0–100 percentile rank.

**Parameters**:
- **formula**: P123 formula in quotes. Use backticks `` ` `` for complex expressions
- **scope**: `#All`, `#Sector`, `#Industry`, `#SubIndustry` (see Scope section below)
- **sort**: `#DESC` (default — higher values → higher rank), `#ASC` (lower values → higher rank, e.g., PE)
- **incl_na**: `#InclNA` (default — include NAs), `#ExclNA` (assign NA to stocks with NA), `#NANeutral` (assign rank 50)
- **sort_style**: `#Top` (default — ties get highest rank, min rank = 100/n), `#Neutral` (ties get average rank, min rank = 0)

```
// Top quintile value (low PE = good → #ASC)
FRank("PEExclXorTTM", #All, #ASC) > 80

// Top decile momentum
FRank(`Close(0)/Close(252)`, #All, #DESC) > 90

// Sector-relative quality
FRank("ROE%TTM", #Sector, #DESC) > 70

// Neutral NA handling
FRank("PEExclXorTTM", #All, #ASC, #NANeutral) > 80

// Complex formula with backticks
FRank(`Eval(IsNA(PEExclXorTTM), Pr2SalesTTM * 15, PEExclXorTTM)`, #All, #ASC) > 75
```

### Composite scores

```
SetVar(@val, FRank("PEExclXorTTM", #All, #ASC))
SetVar(@mom, FRank(`Ret%Chg(252, 21)`, #All, #DESC))
SetVar(@qual, FRank("ROE%TTM", #All, #DESC))
SetVar(@composite, 0.4 * @val + 0.3 * @mom + 0.3 * @qual)
@composite > 70
```

---

## ZScore — Cross-Sectional Z-Score <a name="zscore"></a>

```
ZScore("formula" [, scope=#All, outlier_pct=7.5, na_value=0, max_zscore=3.5])
```

Returns: number of standard deviations from cross-sectional mean (clipped to ±max_zscore).

- **outlier_pct**: trim % from each side (default 7.5%)
- **na_value**: value assigned to NAs (default 0)
- **max_zscore**: clipping boundary (default ±3.5)

```
ZScore("PEExclXorTTM", #All)
ZScore("ROE%TTM", #Sector)

// Combine z-scores
SetVar(@z_pe, -1 * ZScore("PEExclXorTTM", #All))
SetVar(@z_roe, ZScore("ROE%TTM", #All))
@z_pe + @z_roe > 1
```

---

## FOrder, FCount, FSum, FMedian <a name="forder"></a>

| Function | Description |
|----------|-------------|
| `FOrder("formula" [, scope=#All, sort=#DESC, distinct=FALSE, incl_na=#InclNA])` | Returns **position** in sorted array (1, 2, 3...) |
| `FCount("formula" [, scope])` | Count of stocks where formula is true (non-zero) |
| `FSum("formula" [, scope])` | Sum of formula values across scope |
| `FMedian("formula" [, scope, excl_zero])` | Median of formula values across scope |

```
// How many stocks in my sector have PE < 20?
FCount("PEExclXorTTM < 20", #Sector)

// Industry median ROE
FMedian("ROE%TTM", #Industry)

// My ordinal position by market cap (1 = largest)
FOrder("MktCap", #All, #DESC)
```

---

## Aggregate — Cross-Sectional Statistics <a name="aggregate"></a>

```
Aggregate("formula", scope [, method, outlier_pct, outlier_handl, excl_zero, excl_adrs, median_fallback])
```

**Parameters**:
- **method**: `#Avg` (default — simple average), `#CapAvg` (cap-weighted average)
- **scope**: `#All`, `#Sector`, `#Industry`, `#SubIndustry`, `#GroupVar`, `#GroupVar2`, `#Previous1`
- **outlier_pct**: trim % from each side (default 16.5%)
- **outlier_handl**: `#Exclude` (default — remove outliers), `#Winsor` (clip outliers to boundary values)
- **excl_zero**: `TRUE`/`FALSE` (exclude zeros; default FALSE)
- **excl_adrs**: `TRUE`/`FALSE` (exclude ADRs; default TRUE)
- **median_fallback**: when > 0, falls back to simple median if not enough stocks in scope (default 0)

**Note**: P123 does NOT use `#Mean`, `#Median`, `#StdDev`, `#Sum`, `#Count`, `#Min`, `#Max` as Aggregate methods. Use `#Avg` or `#CapAvg`. For other statistics, use `FMedian()`, `FSum()`, `FCount()`, or `ZScore()`.

```
// Industry average PE
Aggregate("PEExclXorTTM", #Industry, #Avg)

// Cap-weighted sector ROE
Aggregate("ROE%TTM", #Sector, #CapAvg)

// With Winsorized outliers
Aggregate("PEExclXorTTM", #All, #Avg, 5, #Winsor)

// Exclude zeros for yield
Aggregate("DivYield%TTM", #Industry, #Avg, 16.5, #Exclude, TRUE)
```

---

## Scope Parameter Values <a name="scope"></a>

Used by `FRank`, `ZScore`, `Aggregate`, `FOrder`, `FCount`, `FSum`, `FMedian`:

| Scope | Description |
|-------|-------------|
| `#All` | Entire universe |
| `#Sector` | GICS sector grouping |
| `#Industry` | GICS industry grouping |
| `#SubIndustry` | GICS sub-industry grouping |
| `#Previous1` | Results from previous rule (screens only) |
| `#GroupVar` | Groups based on `@Group` variable value |
| `#GroupVar2` | Groups based on `@Group2` variable value |

---

## FHist — Historical Time Series <a name="fhist"></a>

**Point-in-time value**:
```
FHist("formula", weeksAgo)
```
Returns the value of `formula` as it was `weeksAgo` weeks in the past.

**Statistical aggregates over historical samples**:

| Function | Description |
|----------|-------------|
| `FHistAvg("formula", samples [, weeks_increment=1, NA_pct=20])` | **Average** of sampled historical values |
| `FHistMax("formula", samples [, weeks_increment=1, NA_pct=20])` | Maximum |
| `FHistMin("formula", samples [, weeks_increment=1, NA_pct=20])` | Minimum |
| `FHistMed("formula", samples [, weeks_increment=1, NA_pct=20])` | Median |
| `FHistSum("formula", samples [, weeks_increment=1, NA_pct=20])` | Sum |
| `FHistStdDev("formula", samples [, weeks_increment=1, NA_pct=20])` | Standard deviation |
| `FHistRelStdDev("formula", samples [, weeks_increment=1, NA_pct=20])` | Relative standard deviation |

**Parameters**:
- **samples**: number of historical observations
- **weeks_increment**: spacing between samples in weeks (default **1** = weekly)
- **NA_pct**: max % NAs allowed before returning NA (default 20%)

```
// Average quarterly ROE over past year (4 samples, 13 weeks apart)
FHistAvg("ROE%TTM", 4, 13)

// Average PE over 5 years (5 annual samples)
FHistAvg("PEExclXorTTM", 5, 52)

// PE value exactly 1 year ago
FHist("PEExclXorTTM", 52)

// 3-year historical max of ROE
FHistMax("ROE%TTM", 156, 1)

// Dividend yield average over 65 weeks (weekly samples)
FHistAvg("DivYield%TTM", 65, 4)
```

---

## FHistRank, FHistRel, FHistZScore — Relative vs History <a name="fhistrank"></a>

Compare current value to its own history:

| Function | Description |
|----------|-------------|
| `FHistRank("formula", samples [, weeks_increment=1, sort=#DESC, sort_style=#Top, NA_value=NA, NA_pct=20])` | Percentile rank of current vs history (0–100) |
| `FHistRel("formula", samples [, weeks_increment=1, NA_value=NA, NA_pct=20])` | Relative position (0–1) vs historical min/max |
| `FHistZScore("formula", samples [, weeks_increment=1, clip=3.5, NA_value=NA, NA_pct=20])` | Z-score of current vs historical values |

```
// Is current PE historically high? (100 = at peak)
FHistRank("PEExclXorTTM", 52, 1)

// Mean reversion: PE historically low
FHistRank("PEExclXorTTM", 104, 1) < 20

// Z-score vs history
FHistZScore("OpMgn%TTM", 52, 1) > 1

// Relative position 0-1
FHistRel("MktCap", 52, 1)
```

---

## Loop Functions — Iteration with CTR <a name="loop"></a>

Loop functions execute a formula multiple times using a `CTR` counter variable:

```
LoopFunction("formula(CTR)", iterations [, start=0, increment=1, ...])
```

### Aggregate Loops

| Function | Description |
|----------|-------------|
| `LoopAvg("formula(CTR)", iterations [, start, increment, noNAs, breakOnNA])` | Average of iterated values |
| `LoopMax(...)` | Maximum |
| `LoopMin(...)` | Minimum |
| `LoopMedian(...)` | Median |
| `LoopSum(...)` | Sum |
| `LoopStdDev(...)` | Standard deviation |
| `LoopRelStdDev(...)` | Relative standard deviation |
| `LoopStreak("formula(CTR)", iterations [, start, increment, streak=#Positive])` | Streak count |

### Relative vs Loop History

| Function | Description |
|----------|-------------|
| `LoopRank("formula(CTR)", iterations [, start, incr, sort, sort_style, NA_value, NA_pct])` | Percentile rank vs iterated values |
| `LoopRel("formula(CTR)", iterations [, start, increment, NA_value, NA_pct])` | Relative position 0–1 |
| `LoopZScore("formula(CTR)", iterations [, start, increment, clip, NA_value, NA_pct])` | Z-score vs iterated values |

```
// Average of quarterly EPS over past 5 years (20 quarters)
LoopAvg("EPSExclXor(CTR, QTR)", 20)

// Number of profitable years out of last 10
LoopSum("Eval(EPSExclXor(CTR, ANN) > 0, 1, 0)", 10)

// Insider buying streak
LoopStreak("InsiderBuySh3M(CTR)", 12, 0, 1, #Positive)

// EPS stability (low relative std dev = stable)
LoopRelStdDev("EPSExclXor(CTR, QTR)", 20) / 100
```

---

## Regression Functions & Statistics <a name="regression"></a>

### Step 1: Compute regression (choose one)

| Function | Description |
|----------|-------------|
| `LinRegVals(y0, y1, ..., y50)` | Regression on Y values (time series) |
| `LinRegXYVals(x0, y0, x1, y1, ..., x50, y50)` | Regression on XY pairs |
| `LinReg("formula(CTR)", iterations [, start, increment])` | Loop-based time series regression |
| `LinRegXY("X-Formula(CTR)", "Y-Formula(CTR)", iterations [, start, increment])` | Loop-based XY regression |

These return `TRUE` if regression succeeds, `FALSE` otherwise.

### Step 2: Access regression statistics

Place these **after** the regression function (to the right or below):

| Stat | Description |
|------|-------------|
| `RegGr%([period=1])` | Growth rate (annualize with period param) |
| `RegEst(offset)` / `EstimateY(offset)` | Y estimate at offset |
| `EstimateXY(X)` | Y estimate for a given X (XY regression) |
| `SurpriseY(offset)` | Surprise (estimated vs actual) |
| `Slope` | Slope of regression line |
| `SlopeConf%` | Confidence = 100 × (1 − SlopePVal) |
| `SlopePVal` | P-value of slope |
| `SlopeSE` | Slope standard error |
| `SlopeTStat` | Slope t-statistic |
| `R` | Correlation coefficient |
| `R2` | Coefficient of determination (R²) |
| `Intercept` | Y-intercept |
| `InterceptSE` | Y-intercept standard error |
| `SE` | Standard error of Y estimate (Sy.x) |
| `Samples` | Number of samples used |

```
// Sales growth trend via regression
LinReg("Sales(CTR, ANN)", 5)
RegGr%()

// EPS regression with confidence check
LinReg("EPSExclXor(CTR, QTR)", 20)
Eval(SlopeConf% > 90, RegGr%(), NA)
```

**Note**: Regression functions require an **Ultimate subscription**.

---

## NodeRank & Ranking Functions <a name="noderank"></a>

| Function | Description |
|----------|-------------|
| `NodeRank("name")` | Rank of a specific node in the **current** ranking system |
| `Rating("RankName")` | Rank from a **different** named ranking system |
| `RatingPos("RankName")` | Rank position from a different ranking system |
| `GetRank("ticker")` | Rank of a specific ticker |
| `GetRankPos("ticker")` | Rank position of a specific ticker |
| `RankPrev(weeksAgo)` | Historical weekly rank |
| `RankPosPrev(weeksAgo)` | Historical weekly rank position |
| `RankBars` | Bars since rank was last calculated |
| `LatestRank` | Latest daily-updated rank |

**Note**: P123 does NOT have `OtherRank()`. Use `Rating("name")` or `RatingPos("name")`.

```
// Use nodes from current ranking system
NodeRank("Value") > 80 AND NodeRank("Quality") > 60

// Compare with another ranking system
Rating("My Quality Rank") > 70
```

---

## AI Factor Functions <a name="aifactor"></a>

```
AIFactor("AI Factor Name", "Predictor Name")
AIFactorValidation("AI Factor Name", "Model Name" [, "dup_id"])
```

```
// Use AI prediction in screen
FRank(`AIFactor("My AI Factor", "lightgbm predictor")`, #All, #DESC) > 80
```

---

## Screen-Only Functions <a name="screen-only"></a>

| Function | Description |
|----------|-------------|
| `IndCount` | Running count of stocks in same industry (must be last rule) |
| `SubIndCount` | Running count in same sub-industry (must be last rule) |
| `ShowCorrel(N)` | Show correlation matrix in report |
| `Screen("ScreenName", top)` | Run another screen; if `top > 0`, return only top N stocks |
| `HoldingsCnt("ListName")` | Count of list stocks that are current holdings |

### Account / Portfolio / Watchlist Holdings

| Function | Description |
|----------|-------------|
| `Account(id1 [, .., id10])` | TRUE if stock is held in account |
| `AccountOpen(id1 [, .., id10])` | Calendar days since position opened |
| `AccountClose(id1 [, .., id10])` | Calendar days since position closed |
| `AccountOpenBar(id1 [, .., id10])` | Bars since position opened |
| `AccountCloseBar(id1 [, .., id10])` | Bars since position closed |
| `Portfolio(...)` | Same syntax for strategies |
| `Watchlist(...)` | Same syntax for watchlists |

**Note**: P123 does NOT have `SectorCount` or `SectCount`. Only `IndCount` and `SubIndCount` exist.

---

## Universe Operations (Strategy) <a name="universe-ops"></a>

These evaluate formulas across the universe, useful in strategy buy/sell rules:

| Function | Description |
|----------|-------------|
| `UnivAvg("criteria", "formula")` | Simple average of formula where criteria is true |
| `UnivCapAvg("criteria", "formula")` | Cap-weighted average |
| `UnivMedian("criteria", "formula")` | Median |
| `UnivMax("criteria", "formula")` | Maximum |
| `UnivMin("criteria", "formula")` | Minimum |
| `UnivSum("criteria", "formula")` | Sum |
| `UnivStdDev("criteria", "formula")` | Standard deviation |
| `UnivCnt("criteria")` | Count stocks passing criteria |
| `UnivExclude("tic1, tic2...")` | Exclude specific tickers |
| `UnivSubset("tic1, tic2...")` | Only include specific tickers |
| `UnivRBICS(rcode, rcode, ...)` | Filter by RBICS classification |

```
// Average PE of SP500 stocks with PE > 0
UnivAvg("PEExclXorTTM > 0", "PEExclXorTTM")

// Number of stocks in universe with positive momentum
UnivCnt("Ret%Chg(252) > 0")
```

---

## Consensus Estimate Functions <a name="consensus"></a>

```
ConsEstMean(cons_item [, period, weekAgo])
ConsEstMedian(cons_item [, period, weekAgo])
ConsEstHi(cons_item [, period, weekAgo])
ConsEstLow(cons_item [, period, weekAgo])
ConsEstCnt(cons_item [, period, weekAgo])
ConsEstStdDev(cons_item [, period, weekAgo])
ConsEstUp(cons_item [, period, weekAgo])
ConsEstDn(cons_item [, period, weekAgo])
ConsEstRSD(cons_item [, period, weekAgo])
```

**cons_item**: `#EPS`, `#Sales`, `#EBITDA`, `#CapEx`, `#FCF`, `#DPS`
**period**: `#CQ`, `#NQ`, `#CY`, `#NY`, `#2Y`
**weekAgo**: 0 (current), 1, 2, ... (for revision tracking)

```
// EPS revision breadth
ConsEstUp(#EPS, #CY) - ConsEstDn(#EPS, #CY)

// Sales estimate trend (current vs 4 weeks ago)
ConsEstMean(#Sales, #CY) / ConsEstMean(#Sales, #CY, 4) - 1
```

### Historical Estimates

| Function | Description |
|----------|-------------|
| `EPSEst(offset, type)` | Historical mean EPS estimate |
| `SalesEst(offset, type)` | Historical mean sales estimate |
| `EPSHistEstCnt(offset, type)` | Historical number of EPS analysts |
| `SalesHistEstCnt(offset, type)` | Historical number of sales analysts |
| `EPSHistEstSD(offset, type)` | Historical EPS estimate std dev |
| `SalesHistEstSD(offset, type)` | Historical sales estimate std dev |

**Note**: P123 does NOT have `HistEstEPS()`, `HistEstSales()`, or `HistEstNumAnalysts()`. Use `EPSEst()`, `SalesEst()`, `EPSHistEstCnt()`, `SalesHistEstCnt()`.

### Recommendation Functions

```
ConsRec(rec_stat [, weekAgo])
```

**rec_stat**: `#Mean`, `#Median`, `#Buy`, `#Outperform`, `#Hold`, `#Underperform`, `#Sell`, `#HoldCnt`, `#Total`

---

## Surprise Functions <a name="surprises"></a>

| Function | Description |
|----------|-------------|
| `EPSSurprise(offset, type)` | EPS surprise (estimate vs actual) |
| `SalesSurprise(offset, type)` | Sales surprise (%) |
| `EPSSUE(offset, type [, constraint])` | Standardized unexpected earnings |
| `SalesSUS(offset, type [, constraint])` | Standardized unexpected sales |

---

## Dividend & Corporate Action Functions <a name="dividends"></a>

### Dividends

| Function / Factor | Description |
|-------------------|-------------|
| `DivPS(offset, type [, div_type, div_dt, cnt_flag])` | Dividends per share in filing period |
| `DivPSDays(days [, offset, div_type, div_dt, cnt_flag])` | Dividends per share in a time period |
| `DaysFromDivEx` | **Days since last ex-dividend date** |
| `Div3YCGr%` | Dividend growth rate 3Y (corporate action data) |
| `Div5YCGr%` | Dividend growth rate 5Y |

**Note**: P123 does NOT have `IndDivA` or `DivDays`. The factor for days since ex-date is `DaysFromDivEx`.

### Splits & Corporate Actions

| Function / Factor | Description |
|-------------------|-------------|
| `Splits(days [, countFlag])` | Compounded split ratio in period |
| `SplitCount(days)` | Number of splits in period |
| `SplitFactor` | Most recent split factor |
| `FutureDivFactor` | Product of all future dividends |
| `FutureSplitFactor` | Product of all future splits |
| `FutureDivSplitFactor` | Product of all future splits and dividends |
| `PastCorpAct(ca_type [, ca_status, lookback, ca_retvalue])` | Past corporate actions query |
| `PendingCorpAct(ca_type [, ca_retvalue])` | Pending corporate actions |

---

## Insider Functions <a name="insider"></a>

All insider functions take a `mo_offset` parameter (0 = current, 1 = one month ago, etc.):

### Shares

| Function | Description |
|----------|-------------|
| `InsiderBuySh1M(mo_offset)` | Shares bought by insiders, past 1 month |
| `InsiderBuySh3M(mo_offset)` | Shares bought, past 3 months |
| `InsiderBuySh6M(mo_offset)` | Shares bought, past 6 months |
| `InsiderBuySh12M(mo_offset)` | Shares bought, past 12 months |
| `InsiderSellSh1M(mo_offset)` | Shares sold, past 1 month |
| `InsiderSellSh3M(mo_offset)` | Shares sold, past 3 months |
| `InsiderSellSh6M(mo_offset)` | Shares sold, past 6 months |
| `InsiderSellSh12M(mo_offset)` | Shares sold, past 12 months |

### Transactions

| Function | Description |
|----------|-------------|
| `InsiderBuyTran1M(mo_offset)` | Buy transactions, past 1 month |
| `InsiderBuyTran3M(mo_offset)` | Buy transactions, past 3 months |
| `InsiderBuyTran6M(mo_offset)` | Buy transactions, past 6 months |
| `InsiderBuyTran12M(mo_offset)` | Buy transactions, past 12 months |
| `InsiderSellTran1M(mo_offset)` | Sell transactions, past 1 month |
| `InsiderSellTran3M(mo_offset)` | Sell transactions, past 3 months |
| `InsiderSellTran6M(mo_offset)` | Sell transactions, past 6 months |
| `InsiderSellTran12M(mo_offset)` | Sell transactions, past 12 months |

### Unique Insiders

| Function | Description |
|----------|-------------|
| `InsiderUniqBuy1M(mo_offset)` | Unique insiders buying, past 1 month |
| `InsiderUniqBuy3M(mo_offset)` | Unique insiders buying, past 3 months |
| `InsiderUniqSell1M(mo_offset)` | Unique insiders selling, past 1 month |
| `InsiderUniqSell3M(mo_offset)` | Unique insiders selling, past 3 months |

**Note**: P123 does NOT have pre-built ratio factors like `InsiderBuySell%3Mo`. Build ratios manually:
```
// Custom insider buy/sell ratio
Eval(InsiderSellSh3M(0) > 0, InsiderBuySh3M(0) / InsiderSellSh3M(0), NA)
```

---

## Institutional Functions <a name="institutional"></a>

All take a `period_offset` parameter (0 = most recent filing, 1 = previous, etc.):

| Function | Description |
|----------|-------------|
| `InstitutionalHolders(period_offset)` | Total number of institutional investors |
| `InstitutionalPctOwn(period_offset)` | % of shares owned by institutions |
| `InstitutionalPctChg(period_offset)` | Net shares changed as % |
| `InstitutionalBuyers(period_offset)` | Number of investors who bought |
| `InstitutionalSellers(period_offset)` | Number of investors who sold |
| `InstitutionalNewBuyers(period_offset)` | Number who opened new positions |
| `InstitutionalClosed(period_offset)` | Number who closed positions |
| `InstitutionalShsHeld(period_offset)` | Total shares held |
| `InstitutionalShsBought(period_offset)` | Shares bought |
| `InstitutionalShsSold(period_offset)` | Shares sold |
| `InstitutionalShsNet(period_offset)` | Net shares (bought − sold) |

**Note**: P123 does NOT have `InstOwn%` or `InstOwnChg%QoQ` as standalone factors. Use `InstitutionalPctOwn(0)` and `InstitutionalPctChg(0)`.

---

## Short Interest <a name="shortinterest"></a>

Short interest factors (pre-built, USA only):

| Factor | Description |
|--------|-------------|
| `SIPM` | Short interest, previous month (millions) |
| `SIPM2` | Short interest, 2 months ago |
| `SIPM3` | Short interest, 3 months ago |
| `SI%Float` | Short interest as % of float |
| `SI%FloatPM` | Short interest % of float, previous month |
| `SI%ShOut` | Short interest as % of shares outstanding |
| `SI%ShOutPM` | Short interest % of shares outstanding, previous month |
| `SI%Chg` | Short interest % change |

**Note**: P123 does NOT have `ShortInt%`, `ShortIntRatio`, `ShortInt%Float`. Use `SI%Float`, `SI%ShOut`, etc.

Short interest data is published twice monthly with ~10 days lag.
