# Ratios & Statistics

Calculated information that combines more than one fundamental data point.

## Valuation

Comparisons between fundamental data points and price.

### Enterprise value to EBITDA

Enterprise value to operating income plus depreciation and amortization.

| Factor | Params | Variant |
|--------|--------|---------|
| `EV2EBITDA()` | offset, type |  |
| `EV2EBITDAQ` |  | Latest Quarter |
| `EV2EBITDAPQ` |  | Previous Quarter |
| `EV2EBITDAPYQ` |  | Previous Quarter 1 Year Ago |
| `EV2EBITDATTM` |  | Trailing 12 Months |
| `EV2EBITDAPTM` |  | Previous Trailing 12 Months |
| `EV2EBITDAA` |  | Latest Year |
| `EV2EBITDAPY` |  | Previous Year |


### Enterprise value to Sales

Enterprise value to sales.

| Factor | Params | Variant |
|--------|--------|---------|
| `EV2Sales()` | offset, type |  |
| `EV2SalesQ` |  | Latest Quarter |
| `EV2SalesPQ` |  | Previous Quarter |
| `EV2SalesPYQ` |  | Previous Quarter 1 Year Ago |
| `EV2SalesTTM` |  | Trailing 12 Months |
| `EV2SalesPTM` |  | Previous Trailing 12 Months |
| `EV2SalesA` |  | Latest Year |
| `EV2SalesPY` |  | Previous Year |


### Price to Book Value

Market value relative to book value of equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2Book()` | offset, type |  |
| `Pr2BookQ` |  | Latest Quarter |
| `Pr2BookPQ` |  | Previous Quarter |
| `Pr2BookPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2BookA` |  | Latest Year |
| `Pr2BookPY` |  | Previous Year |


### Price to Cash Flow

Stock price relative to cash flow per share.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2CashFl()` | offset, type |  |
| `Pr2CashFlQ` |  | Latest Quarter |
| `Pr2CashFlPQ` |  | Previous Quarter |
| `Pr2CashFlPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2CashFlTTM` |  | Trailing 12 Months |
| `Pr2CashFlPTM` |  | Previous Trailing 12 Months |
| `Pr2CashFlA` |  | Latest Year |
| `Pr2CashFlPY` |  | Previous Year |


### Price to Cash Flow Incl R&D (aka Innovation Pr2CF)

Adjusts P/CF ratio by adding R&D expenses back to operating cash flow.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2CFInclRD()` | offset, type |  |
| `Pr2CFInclRDQ` |  | Latest Quarter |
| `Pr2CFInclRDPQ` |  | Previous Quarter |
| `Pr2CFInclRDPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2CFInclRDTTM` |  | Trailing 12 Months |
| `Pr2CFInclRDPTM` |  | Previous Trailing 12 Months |
| `Pr2CFInclRDA` |  | Latest Year |
| `Pr2CFInclRDPY` |  | Previous Year |


### Price to Earnings (other)

Price Earnings Ratio, 5 year High

| Factor | Params | Variant |
|--------|--------|---------|
| `PEHigh` |  | 5 Years |
| `PELow` |  | 5 Years |
| `PERelative` |  | 5 Years |


### Price to Earnings (PE) Excl Xor

Share price relative to earnings per share excluding extraordinary items.

| Factor | Params | Variant |
|--------|--------|---------|
| `PEExclXor()` | offset, type |  |
| `PEExclXorQ` |  | Latest Quarter |
| `PEExclXorPQ` |  | Previous Quarter |
| `PEExclXorPYQ` |  | Previous Quarter 1 Year Ago |
| `PEExclXorTTM` |  | Trailing 12 Months |
| `PEExclXorPTM` |  | Previous Trailing 12 Months |
| `PEExclXorA` |  | Latest Year |
| `PEExclXorPY` |  | Previous Year |


### Price to Earnings (PE) Incl Xor

Share price relative to earnings per share including extraordinary items.

| Factor | Params | Variant |
|--------|--------|---------|
| `PEInclXor()` | offset, type |  |
| `PEInclXorQ` |  | Latest Quarter |
| `PEInclXorPQ` |  | Previous Quarter |
| `PEInclXorPYQ` |  | Previous Quarter 1 Year Ago |
| `PEInclXorTTM` |  | Trailing 12 Months |
| `PEInclXorPTM` |  | Previous Trailing 12 Months |
| `PEInclXorA` |  | Latest Year |
| `PEInclXorPY` |  | Previous Year |


### Price to Earnings Incl R&D (aka Innovation PE)

Adjusts P/E ratio by adding R&D expenses back to earnings.

| Factor | Params | Variant |
|--------|--------|---------|
| `PEInclRD()` | offset, type |  |
| `PEInclRDQ` |  | Latest Quarter |
| `PEInclRDPQ` |  | Previous Quarter |
| `PEInclRDPYQ` |  | Previous Quarter 1 Year Ago |
| `PEInclRDTTM` |  | Trailing 12 Months |
| `PEInclRDPTM` |  | Previous Trailing 12 Months |
| `PEInclRDA` |  | Latest Year |
| `PEInclRDPY` |  | Previous Year |


### Price to Free Cash Flow

Market price per share to free cash flow per share.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2FrCashFl()` | offset, type |  |
| `Pr2FrCashFlQ` |  | Latest Quarter |
| `Pr2FrCashFlPQ` |  | Previous Quarter |
| `Pr2FrCashFlPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2FrCashFlTTM` |  | Trailing 12 Months |
| `Pr2FrCashFlPTM` |  | Previous Trailing 12 Months |
| `Pr2FrCashFlA` |  | Latest Year |
| `Pr2FrCashFlPY` |  | Previous Year |


### Price to Net Free Cash Flow

Market price per share to net free cash flow per share.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2NetFrCashFl()` | offset, type |  |
| `Pr2NetFrCashFlQ` |  | Latest Quarter |
| `Pr2NetFrCashFlPQ` |  | Previous Quarter |
| `Pr2NetFrCashFlPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2NetFrCashFlTTM` |  | Trailing 12 Months |
| `Pr2NetFrCashFlPTM` |  | Previous Trailing 12 Months |
| `Pr2NetFrCashFlA` |  | Latest Year |
| `Pr2NetFrCashFlPY` |  | Previous Year |


### Price to Sales

Market cap to total revenues.

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2Sales()` | offset, type |  |
| `Pr2SalesQ` |  | Latest Quarter |
| `Pr2SalesPQ` |  | Previous Quarter |
| `Pr2SalesPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2SalesTTM` |  | Trailing 12 Months |
| `Pr2SalesPTM` |  | Previous Trailing 12 Months |
| `Pr2SalesA` |  | Latest Year |
| `Pr2SalesPY` |  | Previous Year |


### Price to Tangible Book Value

Stock price to tangible book value per share (common equity minus intangibles).

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2TanBk()` | offset, type |  |
| `Pr2TanBkQ` |  | Latest Quarter |
| `Pr2TanBkPQ` |  | Previous Quarter |
| `Pr2TanBkPYQ` |  | Previous Quarter 1 Year Ago |
| `Pr2TanBkA` |  | Latest Year |
| `Pr2TanBkPY` |  | Previous Year |


### Net Asset Value (NAV)

Monthly NAV average.

bars: 2-12
offset: 0-12

| Factor | Params | Variant |
|--------|--------|---------|
| `NAVAvg()` | bars [, offset] |  |
| `NAVHist()` | offset |  |
| `NAV` |  | Latest |
| `NAVPM` |  | 1 Month Ago |
| `NAVPM2` |  | 2 Months Ago |
| `NAVPM3` |  | 3 Months Ago |


### Net Asset Value (NAV) Discount

Monthly NAV Discount average.

bars: 2-12
offset: 0-12

| Factor | Params | Variant |
|--------|--------|---------|
| `NAVDiscAvg()` | bars [, offset] |  |
| `NAVDiscHist()` | offset |  |
| `NAVDisc` |  | Latest |
| `NAVDiscPM` |  | 1 Month Ago |
| `NAVDiscPM2` |  | 2 Months Ago |
| `NAVDiscPM3` |  | 3 Months Ago |


## Valuation Projected

Other Valuation ratios that involve analyst estimates

### PEG Ratio (long term)

Projected Price/Earnings to Long Term Growth Rate

| Factor | Params | Variant |
|--------|--------|---------|
| `PEGLT` |  | Long Term |
| `PEGLTY` |  | Long Term |


### PEG Ratio (short term)

Price/Earnings to Next Year Growth Rate

| Factor | Params | Variant |
|--------|--------|---------|
| `PEGST` |  | Next Year Growth |
| `PEGSTY` |  | Next Year Growth |


### Price To Earnings (PE) Projected

Current Year Projected P/E Ratio

| Factor | Params | Variant |
|--------|--------|---------|
| `ProjPECurFY` |  | Current Year |
| `ProjPENextFY` |  | Next Fiscal Year |
| `ProjPENTM` |  | Next Twelve Months |


### Price to Sales Projected

Price to Sales Next Twelve Months

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2SalesNTM` |  | Next 12 Months |


## Yield

Factors related to dividend and shareholder yields

### Dividend Yield

Dividend Yield (%) using the Indicated Annual Dividend (IAD).  IAD is a projection of the dividends that will be payed in the next 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `Yield` |  | Current |
| `Yield5YAvg` |  | 5 Years |


### Earnings Yield

The earnings per share for the most recent 12 months divided by market price per share.

| Factor | Params | Variant |
|--------|--------|---------|
| `EarnYield` |  |  |


### EBITDA Yield

The ratio is calculated by dividing the most recent 12 months EBITDA by the current enterprise value.

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAYield` |  |  |


### Free Cash Flow Yield

The ratio is calculated by dividing the most recent trailing twelve months free cash flow by market cap.

| Factor | Params | Variant |
|--------|--------|---------|
| `FCFYield` |  |  |


### Operating Cash Flow Yield

Operating Cash Flow Yield

| Factor | Params | Variant |
|--------|--------|---------|
| `OCFYield` |  |  |


### Operating Income Yield

Operating Income Yield

| Factor | Params | Variant |
|--------|--------|---------|
| `OpIncYield` |  |  |


### Shareholder Yield

Share holder Yield

| Factor | Params | Variant |
|--------|--------|---------|
| `ShareholderYield` |  |  |


## Margins

Functions that return total revenues divided by a data point (usually an income statement line).

### EBITDA Margin

EBITDA as percentage of revenue.

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAMgn%()` | offset, type[, NAHandling] |  |
| `EBITDAMgn%Q` |  | Latest Quarter |
| `EBITDAMgn%PQ` |  | Previous Quarter |
| `EBITDAMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `EBITDAMgn%TTM` |  | Trailing 12 Months |
| `EBITDAMgn%PTM` |  | Previous Trailing 12 Months |
| `EBITDAMgn%A` |  | Latest Year |
| `EBITDAMgn%PY` |  | Previous Year |
| `EBITDAMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `EBITDAMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EBITDAMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `EBITDAMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EBITDAMgn%Gr%A` |  | Growth Annual |
| `EBITDAMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `EBITDAMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `EBITDAMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `EBITDAMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EBITDAMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `EBITDAMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `EBITDAMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `EBITDAMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `EBITDAMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `EBITDAMgn%3YAvg` |  | Three Year Average |
| `EBITDAMgn%5YAvg` |  | Five Year Average |
| `EBITDAMgn%5Y` |  | 5 Years |


### Free Cash Flow Margin

Free cash flow as a percentage of total revenues.

| Factor | Params | Variant |
|--------|--------|---------|
| `FCFLMgn%()` | offset, type[, NAHandling] |  |
| `FCFLMgn%Q` |  | Latest Quarter |
| `FCFLMgn%PQ` |  | Previous Quarter |
| `FCFLMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `FCFLMgn%TTM` |  | Trailing 12 Months |
| `FCFLMgn%PTM` |  | Previous Trailing 12 Months |
| `FCFLMgn%A` |  | Latest Year |
| `FCFLMgn%PY` |  | Previous Year |
| `FCFLMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `FCFLMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `FCFLMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `FCFLMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `FCFLMgn%Gr%A` |  | Growth Annual |
| `FCFLMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `FCFLMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `FCFLMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `FCFLMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `FCFLMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `FCFLMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `FCFLMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `FCFLMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `FCFLMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `FCFLMgn%3YAvg` |  | Three Year Average |
| `FCFLMgn%5YAvg` |  | Five Year Average |


### Gross Profit Margin

Gross profit relative to revenue as a percentage. GMgn% = (Gross Profit ÷ Sales) × 100.

| Factor | Params | Variant |
|--------|--------|---------|
| `GMgn%()` | offset, type[, NAHandling] |  |
| `GMgn%Q` |  | Latest Quarter |
| `GMgn%PQ` |  | Previous Quarter |
| `GMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `GMgn%TTM` |  | Trailing 12 Months |
| `GMgn%PTM` |  | Previous Trailing 12 Months |
| `GMgn%A` |  | Latest Year |
| `GMgn%PY` |  | Previous Year |
| `GMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `GMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `GMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GMgn%Gr%A` |  | Growth Annual |
| `GMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `GMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `GMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `GMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `GMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `GMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `GMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `GMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `GMgn%3YAvg` |  | Three Year Average |
| `GMgn%5YAvg` |  | Five Year Average |
| `GMgn%5Y` |  | 5 Years |


### Gross Profit Margin GAAP

Gross profit relative to revenue as a percentage. GMgn%_GAAP = ((Gross Profit - D&A) ÷ Sales) × 100.

| Factor | Params | Variant |
|--------|--------|---------|
| `GMgn%_GAAP()` | offset, type[, NAHandling] |  |
| `GMgn%_GAAPQ` |  | Latest Quarter |
| `GMgn%_GAAPPQ` |  | Previous Quarter |
| `GMgn%_GAAPPYQ` |  | Previous Quarter 1 Year Ago |
| `GMgn%_GAAPTTM` |  | Trailing 12 Months |
| `GMgn%_GAAPPTM` |  | Previous Trailing 12 Months |
| `GMgn%_GAAPA` |  | Latest Year |
| `GMgn%_GAAPPY` |  | Previous Year |
| `GMgn%_GAAPGr%PQ` |  | Q vs Previous Q Growth |
| `GMgn%_GAAPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GMgn%_GAAPGr%TTM` |  | Trailing Twelve Months Growth |
| `GMgn%_GAAPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GMgn%_GAAPGr%A` |  | Growth Annual |
| `GMgn%_GAAPGr%3Y` |  | Three Year Annualized Growth |
| `GMgn%_GAAPGr%5Y` |  | Five Year Annualized Growth |
| `GMgn%_GAAPGr%10Y` |  | Ten Year Annualized Growth |
| `GMgn%_GAAPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GMgn%_GAAPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `GMgn%_GAAPRegEstANN` |  | Ten Year Regression Estimate |
| `GMgn%_GAAPRegEstTTM` |  | Five Year Regression Estimate |
| `GMgn%_GAAPRegGr%ANN` |  | Ten Year Regression Estimate |
| `GMgn%_GAAPRegGr%TTM` |  | Five Year Regression Growth |
| `GMgn%_GAAP3YAvg` |  | Three Year Average |
| `GMgn%_GAAP5YAvg` |  | Five Year Average |


### Net Free Cash Flow Margin

Net free cash flow as a percentage of total revenues.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetFCFLMgn%()` | offset, type |  |
| `NetFCFLMgn%Q` |  | Latest Quarter |
| `NetFCFLMgn%PQ` |  | Previous Quarter |
| `NetFCFLMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `NetFCFLMgn%TTM` |  | Trailing 12 Months |
| `NetFCFLMgn%PTM` |  | Previous Trailing 12 Months |
| `NetFCFLMgn%A` |  | Latest Year |
| `NetFCFLMgn%PY` |  | Previous Year |
| `NetFCFLMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `NetFCFLMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetFCFLMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `NetFCFLMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetFCFLMgn%Gr%A` |  | Growth Annual |
| `NetFCFLMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `NetFCFLMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `NetFCFLMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `NetFCFLMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetFCFLMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetFCFLMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `NetFCFLMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `NetFCFLMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `NetFCFLMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `NetFCFLMgn%3YAvg` |  | Three Year Average |
| `NetFCFLMgn%5YAvg` |  | Five Year Average |


### Net Profit Margin

Income after taxes as a percentage of total revenue.

| Factor | Params | Variant |
|--------|--------|---------|
| `NPMgn%()` | offset, type[, NAHandling] |  |
| `NPMgn%Q` |  | Latest Quarter |
| `NPMgn%PQ` |  | Previous Quarter |
| `NPMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `NPMgn%TTM` |  | Trailing 12 Months |
| `NPMgn%PTM` |  | Previous Trailing 12 Months |
| `NPMgn%A` |  | Latest Year |
| `NPMgn%PY` |  | Previous Year |
| `NPMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `NPMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NPMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `NPMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NPMgn%Gr%A` |  | Growth Annual |
| `NPMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `NPMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `NPMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `NPMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NPMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `NPMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `NPMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `NPMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `NPMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `NPMgn%PSQ` |  | Quarterly Per Share |
| `NPMgn%PSA` |  | Annual Per Share |
| `NPMgn%%SalesQ` |  | % of Quarterly Sales |
| `NPMgn%%SalesA` |  | % of Annual Sales |
| `NPMgn%%AssetsQ` |  | % of Quarterly Assets |
| `NPMgn%%AssetsA` |  | % of Annual Assets |
| `NPMgn%3YAvg` |  | Three Year Average |
| `NPMgn%5YAvg` |  | Five Year Average |
| `NPMgn%5Y` |  | 5 Years |


### Operating Margin

Percent of revenues after operating expenses.

| Factor | Params | Variant |
|--------|--------|---------|
| `OpMgn%()` | offset, type[, NAHandling] |  |
| `OpMgn%Q` |  | Latest Quarter |
| `OpMgn%PQ` |  | Previous Quarter |
| `OpMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `OpMgn%TTM` |  | Trailing 12 Months |
| `OpMgn%PTM` |  | Previous Trailing 12 Months |
| `OpMgn%A` |  | Latest Year |
| `OpMgn%PY` |  | Previous Year |
| `OpMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `OpMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OpMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `OpMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OpMgn%Gr%A` |  | Growth Annual |
| `OpMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `OpMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `OpMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `OpMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OpMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `OpMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `OpMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `OpMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `OpMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `OpMgn%3YAvg` |  | Three Year Average |
| `OpMgn%5YAvg` |  | Five Year Average |
| `OpMgn%5Y` |  | 5 Years |


### Pretax Margin

Income before taxes as a percentage of total revenue.

| Factor | Params | Variant |
|--------|--------|---------|
| `PTMgn%()` | offset, type[, NAHandling] |  |
| `PTMgn%Q` |  | Latest Quarter |
| `PTMgn%PQ` |  | Previous Quarter |
| `PTMgn%PYQ` |  | Previous Quarter 1 Year Ago |
| `PTMgn%TTM` |  | Trailing 12 Months |
| `PTMgn%PTM` |  | Previous Trailing 12 Months |
| `PTMgn%A` |  | Latest Year |
| `PTMgn%PY` |  | Previous Year |
| `PTMgn%Gr%PQ` |  | Q vs Previous Q Growth |
| `PTMgn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PTMgn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `PTMgn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PTMgn%Gr%A` |  | Growth Annual |
| `PTMgn%Gr%3Y` |  | Three Year Annualized Growth |
| `PTMgn%Gr%5Y` |  | Five Year Annualized Growth |
| `PTMgn%Gr%10Y` |  | Ten Year Annualized Growth |
| `PTMgn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PTMgn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `PTMgn%RegEstANN` |  | Ten Year Regression Estimate |
| `PTMgn%RegEstTTM` |  | Five Year Regression Estimate |
| `PTMgn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `PTMgn%RegGr%TTM` |  | Five Year Regression Growth |
| `PTMgn%3YAvg` |  | Three Year Average |
| `PTMgn%5YAvg` |  | Five Year Average |
| `PTMgn%5Y` |  | 5 Years |


### Selling,Gen,Admin to Sales %

Selling, general and administrative expenses (including R&D) as percentage of total sales.

| Factor | Params | Variant |
|--------|--------|---------|
| `SGA2Sales%()` | offset, type[, NAHandling] |  |
| `SGA2Sales%Q` |  | Latest Quarter |
| `SGA2Sales%PQ` |  | Previous Quarter |
| `SGA2Sales%PYQ` |  | Previous Quarter 1 Year Ago |
| `SGA2Sales%TTM` |  | Trailing 12 Months |
| `SGA2Sales%PTM` |  | Previous Trailing 12 Months |
| `SGA2Sales%A` |  | Latest Year |
| `SGA2Sales%PY` |  | Previous Year |
| `SGA2Sales%Gr%PQ` |  | Q vs Previous Q Growth |
| `SGA2Sales%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SGA2Sales%Gr%TTM` |  | Trailing Twelve Months Growth |
| `SGA2Sales%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SGA2Sales%Gr%A` |  | Growth Annual |
| `SGA2Sales%Gr%3Y` |  | Three Year Annualized Growth |
| `SGA2Sales%Gr%5Y` |  | Five Year Annualized Growth |
| `SGA2Sales%Gr%10Y` |  | Ten Year Annualized Growth |
| `SGA2Sales%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SGA2Sales%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `SGA2Sales%RegEstANN` |  | Ten Year Regression Estimate |
| `SGA2Sales%RegEstTTM` |  | Five Year Regression Estimate |
| `SGA2Sales%RegGr%ANN` |  | Ten Year Regression Estimate |
| `SGA2Sales%RegGr%TTM` |  | Five Year Regression Growth |
| `SGA2Sales%3YAvg` |  | Three Year Average |
| `SGA2Sales%5YAvg` |  | Five Year Average |
| `SGA2Sales%5Y` |  | 5 Years |


## Profitability

Return on Equity, Return on Assets and Return on Investments.

### Return on Assets

Net income before extraordinary items as a percentage of average total assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `ROA%()` | offset, type[, NAHandling] |  |
| `ROA%Q` |  | Latest Quarter |
| `ROA%PQ` |  | Previous Quarter |
| `ROA%PYQ` |  | Previous Quarter 1 Year Ago |
| `ROA%TTM` |  | Trailing 12 Months |
| `ROA%PTM` |  | Previous Trailing 12 Months |
| `ROA%A` |  | Latest Year |
| `ROA%PY` |  | Previous Year |
| `ROA%Gr%PQ` |  | Q vs Previous Q Growth |
| `ROA%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ROA%Gr%TTM` |  | Trailing Twelve Months Growth |
| `ROA%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ROA%Gr%A` |  | Growth Annual |
| `ROA%Gr%3Y` |  | Three Year Annualized Growth |
| `ROA%Gr%5Y` |  | Five Year Annualized Growth |
| `ROA%Gr%10Y` |  | Ten Year Annualized Growth |
| `ROA%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ROA%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `ROA%RegEstANN` |  | Ten Year Regression Estimate |
| `ROA%RegEstTTM` |  | Five Year Regression Estimate |
| `ROA%RegGr%ANN` |  | Ten Year Regression Estimate |
| `ROA%RegGr%TTM` |  | Five Year Regression Growth |
| `ROA%3YAvg` |  | Three Year Average |
| `ROA%5YAvg` |  | Five Year Average |


### Return on Equity

Net income before extraordinary items as a percentage of average common equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `ROE%()` | offset, type[, NAHandling] |  |
| `ROE%Q` |  | Latest Quarter |
| `ROE%PQ` |  | Previous Quarter |
| `ROE%PYQ` |  | Previous Quarter 1 Year Ago |
| `ROE%TTM` |  | Trailing 12 Months |
| `ROE%PTM` |  | Previous Trailing 12 Months |
| `ROE%A` |  | Latest Year |
| `ROE%PY` |  | Previous Year |
| `ROE%Gr%PQ` |  | Q vs Previous Q Growth |
| `ROE%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ROE%Gr%TTM` |  | Trailing Twelve Months Growth |
| `ROE%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ROE%Gr%A` |  | Growth Annual |
| `ROE%Gr%3Y` |  | Three Year Annualized Growth |
| `ROE%Gr%5Y` |  | Five Year Annualized Growth |
| `ROE%Gr%10Y` |  | Ten Year Annualized Growth |
| `ROE%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ROE%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `ROE%RegEstANN` |  | Ten Year Regression Estimate |
| `ROE%RegEstTTM` |  | Five Year Regression Estimate |
| `ROE%RegGr%ANN` |  | Ten Year Regression Estimate |
| `ROE%RegGr%TTM` |  | Five Year Regression Growth |
| `ROE%3YAvg` |  | Three Year Average |
| `ROE%5YAvg` |  | Five Year Average |


### Return on Investment

Net income plus after-tax interest expense as a percentage of average total capital.

| Factor | Params | Variant |
|--------|--------|---------|
| `ROI%()` | offset, type[, NAHandling] |  |
| `ROI%Q` |  | Latest Quarter |
| `ROI%PQ` |  | Previous Quarter |
| `ROI%PYQ` |  | Previous Quarter 1 Year Ago |
| `ROI%TTM` |  | Trailing 12 Months |
| `ROI%PTM` |  | Previous Trailing 12 Months |
| `ROI%A` |  | Latest Year |
| `ROI%PY` |  | Previous Year |
| `ROI%Gr%PQ` |  | Q vs Previous Q Growth |
| `ROI%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ROI%Gr%TTM` |  | Trailing Twelve Months Growth |
| `ROI%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ROI%Gr%A` |  | Growth Annual |
| `ROI%Gr%3Y` |  | Three Year Annualized Growth |
| `ROI%Gr%5Y` |  | Five Year Annualized Growth |
| `ROI%Gr%10Y` |  | Ten Year Annualized Growth |
| `ROI%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ROI%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `ROI%RegEstANN` |  | Ten Year Regression Estimate |
| `ROI%RegEstTTM` |  | Five Year Regression Estimate |
| `ROI%RegGr%ANN` |  | Ten Year Regression Estimate |
| `ROI%RegGr%TTM` |  | Five Year Regression Growth |
| `ROI%3YAvg` |  | Three Year Average |
| `ROI%5YAvg` |  | Five Year Average |


## Per Share Ratios

Fundamental line items divided by the number of fully diluted shares.

### Book Value Per Share

The per-share value of common equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `BVPS()` | offset, type[, NAHandling] |  |
| `BVPSQ` |  | Latest Quarter |
| `BVPSPQ` |  | Previous Quarter |
| `BVPSPYQ` |  | Previous Quarter 1 Year Ago |
| `BVPSTTM` |  | Trailing 12 Months |
| `BVPSPTM` |  | Previous Trailing 12 Months |
| `BVPSA` |  | Latest Year |
| `BVPSPY` |  | Previous Year |
| `BVPSGr%PQ` |  | Q vs Previous Q Growth |
| `BVPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `BVPSGr%TTM` |  | Trailing Twelve Months Growth |
| `BVPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `BVPSGr%A` |  | Growth Annual |
| `BVPSGr%3Y` |  | Three Year Annualized Growth |
| `BVPSGr%5Y` |  | Five Year Annualized Growth |
| `BVPSGr%10Y` |  | Ten Year Annualized Growth |
| `BVPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `BVPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `BVPSRegEstANN` |  | Ten Year Regression Estimate |
| `BVPSRegEstTTM` |  | Five Year Regression Estimate |
| `BVPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `BVPSRegGr%TTM` |  | Five Year Regression Growth |
| `BVPS3YAvg` |  | Three Year Average |
| `BVPS5YAvg` |  | Five Year Average |


### Capital Expenditures (CapEx) Per Share

Capital expenditures divided by shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `CapExPS()` | offset, type[, NAHandling] |  |
| `CapExPSQ` |  | Latest Quarter |
| `CapExPSPQ` |  | Previous Quarter |
| `CapExPSPYQ` |  | Previous Quarter 1 Year Ago |
| `CapExPSTTM` |  | Trailing 12 Months |
| `CapExPSPTM` |  | Previous Trailing 12 Months |
| `CapExPSA` |  | Latest Year |
| `CapExPSPY` |  | Previous Year |
| `CapExPSGr%PQ` |  | Q vs Previous Q Growth |
| `CapExPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CapExPSGr%TTM` |  | Trailing Twelve Months Growth |
| `CapExPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CapExPSGr%A` |  | Growth Annual |
| `CapExPSGr%3Y` |  | Three Year Annualized Growth |
| `CapExPSGr%5Y` |  | Five Year Annualized Growth |
| `CapExPSGr%10Y` |  | Ten Year Annualized Growth |
| `CapExPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CapExPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CapExPSRegEstANN` |  | Ten Year Regression Estimate |
| `CapExPSRegEstTTM` |  | Five Year Regression Estimate |
| `CapExPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `CapExPSRegGr%TTM` |  | Five Year Regression Growth |
| `CapExPS3YAvg` |  | Three Year Average |
| `CapExPS5YAvg` |  | Five Year Average |


### Cash Flow Per Share

Cash Flow ÷ Fully-Diluted Average Shares Outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `CashFlPS()` | offset, type[, NAHandling] |  |
| `CashFlPSQ` |  | Latest Quarter |
| `CashFlPSPQ` |  | Previous Quarter |
| `CashFlPSPYQ` |  | Previous Quarter 1 Year Ago |
| `CashFlPSTTM` |  | Trailing 12 Months |
| `CashFlPSPTM` |  | Previous Trailing 12 Months |
| `CashFlPSA` |  | Latest Year |
| `CashFlPSPY` |  | Previous Year |
| `CashFlPSGr%PQ` |  | Q vs Previous Q Growth |
| `CashFlPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashFlPSGr%TTM` |  | Trailing Twelve Months Growth |
| `CashFlPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashFlPSGr%A` |  | Growth Annual |
| `CashFlPSGr%3Y` |  | Three Year Annualized Growth |
| `CashFlPSGr%5Y` |  | Five Year Annualized Growth |
| `CashFlPSGr%10Y` |  | Ten Year Annualized Growth |
| `CashFlPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashFlPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashFlPSRegEstANN` |  | Ten Year Regression Estimate |
| `CashFlPSRegEstTTM` |  | Five Year Regression Estimate |
| `CashFlPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashFlPSRegGr%TTM` |  | Five Year Regression Growth |
| `CashFlPS3YAvg` |  | Three Year Average |
| `CashFlPS5YAvg` |  | Five Year Average |


### Cash Per Share

Total cash plus short-term investments divided by fully-diluted shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `CashPS()` | offset, type[, NAHandling] |  |
| `CashPSQ` |  | Latest Quarter |
| `CashPSPQ` |  | Previous Quarter |
| `CashPSPYQ` |  | Previous Quarter 1 Year Ago |
| `CashPSTTM` |  | Trailing 12 Months |
| `CashPSPTM` |  | Previous Trailing 12 Months |
| `CashPSA` |  | Latest Year |
| `CashPSPY` |  | Previous Year |
| `CashPSGr%PQ` |  | Q vs Previous Q Growth |
| `CashPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashPSGr%TTM` |  | Trailing Twelve Months Growth |
| `CashPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashPSGr%A` |  | Growth Annual |
| `CashPSGr%3Y` |  | Three Year Annualized Growth |
| `CashPSGr%5Y` |  | Five Year Annualized Growth |
| `CashPSGr%10Y` |  | Ten Year Annualized Growth |
| `CashPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashPSRegEstANN` |  | Ten Year Regression Estimate |
| `CashPSRegEstTTM` |  | Five Year Regression Estimate |
| `CashPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashPSRegGr%TTM` |  | Five Year Regression Growth |
| `CashPS3YAvg` |  | Three Year Average |
| `CashPS5YAvg` |  | Five Year Average |


### Earnings Per Share (EPS) Excl Xor

Earnings per share without extraordinary expenses.

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSExclXor()` | offset, type[, NAHandling] |  |
| `EPSExclXorQ` |  | Latest Quarter |
| `EPSExclXorPQ` |  | Previous Quarter |
| `EPSExclXorPYQ` |  | Previous Quarter 1 Year Ago |
| `EPSExclXorTTM` |  | Trailing 12 Months |
| `EPSExclXorPTM` |  | Previous Trailing 12 Months |
| `EPSExclXorA` |  | Latest Year |
| `EPSExclXorPY` |  | Previous Year |
| `EPSExclXorGr%PQ` |  | Q vs Previous Q Growth |
| `EPSExclXorGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EPSExclXorGr%TTM` |  | Trailing Twelve Months Growth |
| `EPSExclXorGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EPSExclXorGr%A` |  | Growth Annual |
| `EPSExclXorGr%3Y` |  | Three Year Annualized Growth |
| `EPSExclXorGr%5Y` |  | Five Year Annualized Growth |
| `EPSExclXorGr%10Y` |  | Ten Year Annualized Growth |
| `EPSExclXorRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EPSExclXorRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EPSExclXorRegEstANN` |  | Ten Year Regression Estimate |
| `EPSExclXorRegEstTTM` |  | Five Year Regression Estimate |
| `EPSExclXorRegGr%ANN` |  | Ten Year Regression Estimate |
| `EPSExclXorRegGr%TTM` |  | Five Year Regression Growth |
| `EPSExclXor3YAvg` |  | Three Year Average |
| `EPSExclXor5YAvg` |  | Five Year Average |


### Earnings Per Share (EPS) Incl Xor

Earnings per share with all expenses including extraordinary items.

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSInclXor()` | offset, type[, NAHandling] |  |
| `EPSInclXorQ` |  | Latest Quarter |
| `EPSInclXorPQ` |  | Previous Quarter |
| `EPSInclXorPYQ` |  | Previous Quarter 1 Year Ago |
| `EPSInclXorTTM` |  | Trailing 12 Months |
| `EPSInclXorPTM` |  | Previous Trailing 12 Months |
| `EPSInclXorA` |  | Latest Year |
| `EPSInclXorPY` |  | Previous Year |
| `EPSInclXorGr%PQ` |  | Q vs Previous Q Growth |
| `EPSInclXorGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EPSInclXorGr%TTM` |  | Trailing Twelve Months Growth |
| `EPSInclXorGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EPSInclXorGr%A` |  | Growth Annual |
| `EPSInclXorGr%3Y` |  | Three Year Annualized Growth |
| `EPSInclXorGr%5Y` |  | Five Year Annualized Growth |
| `EPSInclXorGr%10Y` |  | Ten Year Annualized Growth |
| `EPSInclXorRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EPSInclXorRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EPSInclXorRegEstANN` |  | Ten Year Regression Estimate |
| `EPSInclXorRegEstTTM` |  | Five Year Regression Estimate |
| `EPSInclXorRegGr%ANN` |  | Ten Year Regression Estimate |
| `EPSInclXorRegGr%TTM` |  | Five Year Regression Growth |
| `EPSInclXor3YAvg` |  | Three Year Average |
| `EPSInclXor5YAvg` |  | Five Year Average |


### EBITDA Per Share

Earnings before interest, taxes, depreciation and amortization on a per-share basis.

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAPS()` | offset, type[, NAHandling] |  |
| `EBITDAPSQ` |  | Latest Quarter |
| `EBITDAPSPQ` |  | Previous Quarter |
| `EBITDAPSPYQ` |  | Previous Quarter 1 Year Ago |
| `EBITDAPSTTM` |  | Trailing 12 Months |
| `EBITDAPSPTM` |  | Previous Trailing 12 Months |
| `EBITDAPSA` |  | Latest Year |
| `EBITDAPSPY` |  | Previous Year |
| `EBITDAPSGr%PQ` |  | Q vs Previous Q Growth |
| `EBITDAPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EBITDAPSGr%TTM` |  | Trailing Twelve Months Growth |
| `EBITDAPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EBITDAPSGr%A` |  | Growth Annual |
| `EBITDAPSGr%3Y` |  | Three Year Annualized Growth |
| `EBITDAPSGr%5Y` |  | Five Year Annualized Growth |
| `EBITDAPSGr%10Y` |  | Ten Year Annualized Growth |
| `EBITDAPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EBITDAPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EBITDAPSRegEstANN` |  | Ten Year Regression Estimate |
| `EBITDAPSRegEstTTM` |  | Five Year Regression Estimate |
| `EBITDAPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `EBITDAPSRegGr%TTM` |  | Five Year Regression Growth |
| `EBITDAPS3YAvg` |  | Three Year Average |
| `EBITDAPS5YAvg` |  | Five Year Average |


### Free Cash Flow Per Share

Free cash flow divided by fully-diluted average shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `FCFPS()` | offset, type[, NAHandling] |  |
| `FCFPSQ` |  | Latest Quarter |
| `FCFPSPQ` |  | Previous Quarter |
| `FCFPSPYQ` |  | Previous Quarter 1 Year Ago |
| `FCFPSTTM` |  | Trailing 12 Months |
| `FCFPSPTM` |  | Previous Trailing 12 Months |
| `FCFPSA` |  | Latest Year |
| `FCFPSPY` |  | Previous Year |
| `FCFPSGr%PQ` |  | Q vs Previous Q Growth |
| `FCFPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `FCFPSGr%TTM` |  | Trailing Twelve Months Growth |
| `FCFPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `FCFPSGr%A` |  | Growth Annual |
| `FCFPSGr%3Y` |  | Three Year Annualized Growth |
| `FCFPSGr%5Y` |  | Five Year Annualized Growth |
| `FCFPSGr%10Y` |  | Ten Year Annualized Growth |
| `FCFPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `FCFPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `FCFPSRegEstANN` |  | Ten Year Regression Estimate |
| `FCFPSRegEstTTM` |  | Five Year Regression Estimate |
| `FCFPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `FCFPSRegGr%TTM` |  | Five Year Regression Growth |
| `FCFPS3YAvg` |  | Three Year Average |
| `FCFPS5YAvg` |  | Five Year Average |


### Net Free Cash Flow Per Share

Net Free Cash Flow per Share is quarterly net free cash flow divided by fully-diluted average shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetFCFPS()` | offset, type |  |
| `NetFCFPSQ` |  | Latest Quarter |
| `NetFCFPSPQ` |  | Previous Quarter |
| `NetFCFPSPYQ` |  | Previous Quarter 1 Year Ago |
| `NetFCFPSTTM` |  | Trailing 12 Months |
| `NetFCFPSPTM` |  | Previous Trailing 12 Months |
| `NetFCFPSA` |  | Latest Year |
| `NetFCFPSPY` |  | Previous Year |
| `NetFCFPSGr%PQ` |  | Q vs Previous Q Growth |
| `NetFCFPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetFCFPSGr%TTM` |  | Trailing Twelve Months Growth |
| `NetFCFPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetFCFPSGr%A` |  | Growth Annual |
| `NetFCFPSGr%3Y` |  | Three Year Annualized Growth |
| `NetFCFPSGr%5Y` |  | Five Year Annualized Growth |
| `NetFCFPSGr%10Y` |  | Ten Year Annualized Growth |
| `NetFCFPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetFCFPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetFCFPSRegEstANN` |  | Ten Year Regression Estimate |
| `NetFCFPSRegEstTTM` |  | Five Year Regression Estimate |
| `NetFCFPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetFCFPSRegGr%TTM` |  | Five Year Regression Growth |
| `NetFCFPS3YAvg` |  | Three Year Average |
| `NetFCFPS5YAvg` |  | Five Year Average |


### Operating Cashflow Per Share

Operating Cashflow Per Share.

| Factor | Params | Variant |
|--------|--------|---------|
| `OCFPS()` | offset, type[, NAHandling] |  |
| `OCFPSQ` |  | Latest Quarter |
| `OCFPSPQ` |  | Previous Quarter |
| `OCFPSPYQ` |  | Previous Quarter 1 Year Ago |
| `OCFPSTTM` |  | Trailing 12 Months |
| `OCFPSPTM` |  | Previous Trailing 12 Months |
| `OCFPSA` |  | Latest Year |
| `OCFPSPY` |  | Previous Year |
| `OCFPSGr%PQ` |  | Q vs Previous Q Growth |
| `OCFPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OCFPSGr%TTM` |  | Trailing Twelve Months Growth |
| `OCFPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OCFPSGr%A` |  | Growth Annual |
| `OCFPSGr%3Y` |  | Three Year Annualized Growth |
| `OCFPSGr%5Y` |  | Five Year Annualized Growth |
| `OCFPSGr%10Y` |  | Ten Year Annualized Growth |
| `OCFPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OCFPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OCFPSRegEstANN` |  | Ten Year Regression Estimate |
| `OCFPSRegEstTTM` |  | Five Year Regression Estimate |
| `OCFPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `OCFPSRegGr%TTM` |  | Five Year Regression Growth |
| `OCFPS3YAvg` |  | Three Year Average |
| `OCFPS5YAvg` |  | Five Year Average |


### Operating Income Per Share

Operating income divided by fully-diluted average shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `OpIncPS()` | offset, type[, NAHandling] |  |
| `OpIncPSQ` |  | Latest Quarter |
| `OpIncPSPQ` |  | Previous Quarter |
| `OpIncPSPYQ` |  | Previous Quarter 1 Year Ago |
| `OpIncPSTTM` |  | Trailing 12 Months |
| `OpIncPSPTM` |  | Previous Trailing 12 Months |
| `OpIncPSA` |  | Latest Year |
| `OpIncPSPY` |  | Previous Year |
| `OpIncPSGr%PQ` |  | Q vs Previous Q Growth |
| `OpIncPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OpIncPSGr%TTM` |  | Trailing Twelve Months Growth |
| `OpIncPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OpIncPSGr%A` |  | Growth Annual |
| `OpIncPSGr%3Y` |  | Three Year Annualized Growth |
| `OpIncPSGr%5Y` |  | Five Year Annualized Growth |
| `OpIncPSGr%10Y` |  | Ten Year Annualized Growth |
| `OpIncPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OpIncPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OpIncPSRegEstANN` |  | Ten Year Regression Estimate |
| `OpIncPSRegEstTTM` |  | Five Year Regression Estimate |
| `OpIncPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `OpIncPSRegGr%TTM` |  | Five Year Regression Growth |
| `OpIncPS3YAvg` |  | Three Year Average |
| `OpIncPS5YAvg` |  | Five Year Average |


### Sales (Revenues) Per Share

Total revenue divided by fully-diluted average shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesPS()` | offset, type[, NAHandling] |  |
| `SalesPSQ` |  | Latest Quarter |
| `SalesPSPQ` |  | Previous Quarter |
| `SalesPSPYQ` |  | Previous Quarter 1 Year Ago |
| `SalesPSTTM` |  | Trailing 12 Months |
| `SalesPSPTM` |  | Previous Trailing 12 Months |
| `SalesPSA` |  | Latest Year |
| `SalesPSPY` |  | Previous Year |
| `SalesPSGr%PQ` |  | Q vs Previous Q Growth |
| `SalesPSGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SalesPSGr%TTM` |  | Trailing Twelve Months Growth |
| `SalesPSGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SalesPSGr%A` |  | Growth Annual |
| `SalesPSGr%3Y` |  | Three Year Annualized Growth |
| `SalesPSGr%5Y` |  | Five Year Annualized Growth |
| `SalesPSGr%10Y` |  | Ten Year Annualized Growth |
| `SalesPSRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SalesPSRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SalesPSRegEstANN` |  | Ten Year Regression Estimate |
| `SalesPSRegEstTTM` |  | Five Year Regression Estimate |
| `SalesPSRegGr%ANN` |  | Ten Year Regression Estimate |
| `SalesPSRegGr%TTM` |  | Five Year Regression Growth |
| `SalesPS3YAvg` |  | Three Year Average |
| `SalesPS5YAvg` |  | Five Year Average |


## Efficiency

Turnover and per-employee ratios.

### Asset Turnover

Revenue divided by the average total assets for the same period.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstTurn()` | offset, type[, NAHandling] |  |
| `AstTurnQ` |  | Latest Quarter |
| `AstTurnPQ` |  | Previous Quarter |
| `AstTurnPYQ` |  | Previous Quarter 1 Year Ago |
| `AstTurnTTM` |  | Trailing 12 Months |
| `AstTurnPTM` |  | Previous Trailing 12 Months |
| `AstTurnA` |  | Latest Year |
| `AstTurnPY` |  | Previous Year |
| `AstTurnGr%PQ` |  | Q vs Previous Q Growth |
| `AstTurnGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstTurnGr%TTM` |  | Trailing Twelve Months Growth |
| `AstTurnGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstTurnGr%A` |  | Growth Annual |
| `AstTurnGr%3Y` |  | Three Year Annualized Growth |
| `AstTurnGr%5Y` |  | Five Year Annualized Growth |
| `AstTurnGr%10Y` |  | Ten Year Annualized Growth |
| `AstTurnRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstTurnRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstTurnRegEstANN` |  | Ten Year Regression Estimate |
| `AstTurnRegEstTTM` |  | Five Year Regression Estimate |
| `AstTurnRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstTurnRegGr%TTM` |  | Five Year Regression Growth |
| `AstTurnPSQ` |  | Quarterly Per Share |
| `AstTurnPSA` |  | Annual Per Share |
| `AstTurn%SalesQ` |  | % of Quarterly Sales |
| `AstTurn%SalesA` |  | % of Annual Sales |
| `AstTurn%AssetsQ` |  | % of Quarterly Assets |
| `AstTurn%AssetsA` |  | % of Annual Assets |
| `AstTurn3YAvg` |  | Three Year Average |
| `AstTurn5YAvg` |  | Five Year Average |


### Income Per Employee

Income per Employee.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncPerEmp()` | offset, type[, NAHandling] |  |
| `IncPerEmpQ` |  | Latest Quarter |
| `IncPerEmpPQ` |  | Previous Quarter |
| `IncPerEmpPYQ` |  | Previous Quarter 1 Year Ago |
| `IncPerEmpTTM` |  | Trailing 12 Months |
| `IncPerEmpPTM` |  | Previous Trailing 12 Months |
| `IncPerEmpA` |  | Latest Year |
| `IncPerEmpPY` |  | Previous Year |
| `IncPerEmpGr%PQ` |  | Q vs Previous Q Growth |
| `IncPerEmpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncPerEmpGr%TTM` |  | Trailing Twelve Months Growth |
| `IncPerEmpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncPerEmpGr%A` |  | Growth Annual |
| `IncPerEmpGr%3Y` |  | Three Year Annualized Growth |
| `IncPerEmpGr%5Y` |  | Five Year Annualized Growth |
| `IncPerEmpGr%10Y` |  | Ten Year Annualized Growth |
| `IncPerEmpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncPerEmpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncPerEmpRegEstANN` |  | Ten Year Regression Estimate |
| `IncPerEmpRegEstTTM` |  | Five Year Regression Estimate |
| `IncPerEmpRegGr%ANN` |  | Ten Year Regression Estimate |
| `IncPerEmpRegGr%TTM` |  | Five Year Regression Growth |
| `IncPerEmp3YAvg` |  | Three Year Average |
| `IncPerEmp5YAvg` |  | Five Year Average |


### Inventory Turnover

Measure of how quickly inventory is sold.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvTurn()` | offset, type[, NAHandling] |  |
| `InvTurnQ` |  | Latest Quarter |
| `InvTurnPQ` |  | Previous Quarter |
| `InvTurnPYQ` |  | Previous Quarter 1 Year Ago |
| `InvTurnTTM` |  | Trailing 12 Months |
| `InvTurnPTM` |  | Previous Trailing 12 Months |
| `InvTurnA` |  | Latest Year |
| `InvTurnPY` |  | Previous Year |
| `InvTurnGr%PQ` |  | Q vs Previous Q Growth |
| `InvTurnGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvTurnGr%TTM` |  | Trailing Twelve Months Growth |
| `InvTurnGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvTurnGr%A` |  | Growth Annual |
| `InvTurnGr%3Y` |  | Three Year Annualized Growth |
| `InvTurnGr%5Y` |  | Five Year Annualized Growth |
| `InvTurnGr%10Y` |  | Ten Year Annualized Growth |
| `InvTurnRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvTurnRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvTurnRegEstANN` |  | Ten Year Regression Estimate |
| `InvTurnRegEstTTM` |  | Five Year Regression Estimate |
| `InvTurnRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvTurnRegGr%TTM` |  | Five Year Regression Growth |
| `InvTurnPSQ` |  | Quarterly Per Share |
| `InvTurnPSA` |  | Annual Per Share |
| `InvTurn%SalesQ` |  | % of Quarterly Sales |
| `InvTurn%SalesA` |  | % of Annual Sales |
| `InvTurn%AssetsQ` |  | % of Quarterly Assets |
| `InvTurn%AssetsA` |  | % of Annual Assets |
| `InvTurn3YAvg` |  | Three Year Average |
| `InvTurn5YAvg` |  | Five Year Average |


### Receivables Turnover

Measure of how efficiently a company collects receivables.

| Factor | Params | Variant |
|--------|--------|---------|
| `RecTurn()` | offset, type[, NAHandling] |  |
| `RecTurnQ` |  | Latest Quarter |
| `RecTurnPQ` |  | Previous Quarter |
| `RecTurnPYQ` |  | Previous Quarter 1 Year Ago |
| `RecTurnTTM` |  | Trailing 12 Months |
| `RecTurnPTM` |  | Previous Trailing 12 Months |
| `RecTurnA` |  | Latest Year |
| `RecTurnPY` |  | Previous Year |
| `RecTurnGr%PQ` |  | Q vs Previous Q Growth |
| `RecTurnGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `RecTurnGr%TTM` |  | Trailing Twelve Months Growth |
| `RecTurnGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `RecTurnGr%A` |  | Growth Annual |
| `RecTurnGr%3Y` |  | Three Year Annualized Growth |
| `RecTurnGr%5Y` |  | Five Year Annualized Growth |
| `RecTurnGr%10Y` |  | Ten Year Annualized Growth |
| `RecTurnRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `RecTurnRSD%TTM` |  | Five Year Relative Standard Deviation |
| `RecTurnRegEstANN` |  | Ten Year Regression Estimate |
| `RecTurnRegEstTTM` |  | Five Year Regression Estimate |
| `RecTurnRegGr%ANN` |  | Ten Year Regression Estimate |
| `RecTurnRegGr%TTM` |  | Five Year Regression Growth |
| `RecTurnPSQ` |  | Quarterly Per Share |
| `RecTurnPSA` |  | Annual Per Share |
| `RecTurn%SalesQ` |  | % of Quarterly Sales |
| `RecTurn%SalesA` |  | % of Annual Sales |
| `RecTurn%AssetsQ` |  | % of Quarterly Assets |
| `RecTurn%AssetsA` |  | % of Annual Assets |
| `RecTurn3YAvg` |  | Three Year Average |
| `RecTurn5YAvg` |  | Five Year Average |


### Sales Per Employee

Sales Per Employee.

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesPerEmp()` | offset, type[, NAHandling] |  |
| `SalesPerEmpQ` |  | Latest Quarter |
| `SalesPerEmpPQ` |  | Previous Quarter |
| `SalesPerEmpPYQ` |  | Previous Quarter 1 Year Ago |
| `SalesPerEmpTTM` |  | Trailing 12 Months |
| `SalesPerEmpPTM` |  | Previous Trailing 12 Months |
| `SalesPerEmpA` |  | Latest Year |
| `SalesPerEmpPY` |  | Previous Year |
| `SalesPerEmpGr%PQ` |  | Q vs Previous Q Growth |
| `SalesPerEmpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SalesPerEmpGr%TTM` |  | Trailing Twelve Months Growth |
| `SalesPerEmpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SalesPerEmpGr%A` |  | Growth Annual |
| `SalesPerEmpGr%3Y` |  | Three Year Annualized Growth |
| `SalesPerEmpGr%5Y` |  | Five Year Annualized Growth |
| `SalesPerEmpGr%10Y` |  | Ten Year Annualized Growth |
| `SalesPerEmpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SalesPerEmpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SalesPerEmpRegEstANN` |  | Ten Year Regression Estimate |
| `SalesPerEmpRegEstTTM` |  | Five Year Regression Estimate |
| `SalesPerEmpRegGr%ANN` |  | Ten Year Regression Estimate |
| `SalesPerEmpRegGr%TTM` |  | Five Year Regression Growth |
| `SalesPerEmp3YAvg` |  | Three Year Average |
| `SalesPerEmp5YAvg` |  | Five Year Average |


### Sales, General and Administrative Expense to Gross Profit

Indirect costs as percentage of gross profit.

| Factor | Params | Variant |
|--------|--------|---------|
| `SGA2GP()` | offset, type[, NAHandling] |  |
| `SGA2GPQ` |  | Latest Quarter |
| `SGA2GPPQ` |  | Previous Quarter |
| `SGA2GPPYQ` |  | Previous Quarter 1 Year Ago |
| `SGA2GPTTM` |  | Trailing 12 Months |
| `SGA2GPPTM` |  | Previous Trailing 12 Months |
| `SGA2GPA` |  | Latest Year |
| `SGA2GPPY` |  | Previous Year |
| `SGA2GPGr%PQ` |  | Q vs Previous Q Growth |
| `SGA2GPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SGA2GPGr%TTM` |  | Trailing Twelve Months Growth |
| `SGA2GPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SGA2GPGr%A` |  | Growth Annual |
| `SGA2GPGr%3Y` |  | Three Year Annualized Growth |
| `SGA2GPGr%5Y` |  | Five Year Annualized Growth |
| `SGA2GPGr%10Y` |  | Ten Year Annualized Growth |
| `SGA2GPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SGA2GPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SGA2GPRegEstANN` |  | Ten Year Regression Estimate |
| `SGA2GPRegEstTTM` |  | Five Year Regression Estimate |
| `SGA2GPRegGr%ANN` |  | Ten Year Regression Estimate |
| `SGA2GPRegGr%TTM` |  | Five Year Regression Growth |
| `SGA2GPPSQ` |  | Quarterly Per Share |
| `SGA2GPPSA` |  | Annual Per Share |
| `SGA2GP%SalesQ` |  | % of Quarterly Sales |
| `SGA2GP%SalesA` |  | % of Annual Sales |
| `SGA2GP%AssetsQ` |  | % of Quarterly Assets |
| `SGA2GP%AssetsA` |  | % of Annual Assets |
| `SGA2GP3YAvg` |  | Three Year Average |
| `SGA2GP5YAvg` |  | Five Year Average |


## Financial Strength

Quality tests, particularly relating to debt or dividend payout.

### Current Ratio

Measures company's ability to pay short-term obligations using short-term assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `CurRatio()` | offset, type[, NAHandling] |  |
| `CurRatioQ` |  | Latest Quarter |
| `CurRatioPQ` |  | Previous Quarter |
| `CurRatioPYQ` |  | Previous Quarter 1 Year Ago |
| `CurRatioTTM` |  | Trailing 12 Months |
| `CurRatioPTM` |  | Previous Trailing 12 Months |
| `CurRatioA` |  | Latest Year |
| `CurRatioPY` |  | Previous Year |
| `CurRatioGr%PQ` |  | Q vs Previous Q Growth |
| `CurRatioGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CurRatioGr%TTM` |  | Trailing Twelve Months Growth |
| `CurRatioGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CurRatioGr%A` |  | Growth Annual |
| `CurRatioGr%3Y` |  | Three Year Annualized Growth |
| `CurRatioGr%5Y` |  | Five Year Annualized Growth |
| `CurRatioGr%10Y` |  | Ten Year Annualized Growth |
| `CurRatioRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CurRatioRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CurRatioRegEstANN` |  | Ten Year Regression Estimate |
| `CurRatioRegEstTTM` |  | Five Year Regression Estimate |
| `CurRatioRegGr%ANN` |  | Ten Year Regression Estimate |
| `CurRatioRegGr%TTM` |  | Five Year Regression Growth |
| `CurRatio3YAvg` |  | Three Year Average |
| `CurRatio5YAvg` |  | Five Year Average |


### Debt Service to Net Income

Ratio of interest expense relative to earnings.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtS2NI()` | offset, type[, NAHandling] |  |
| `DbtS2NIQ` |  | Latest Quarter |
| `DbtS2NIPQ` |  | Previous Quarter |
| `DbtS2NIPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtS2NITTM` |  | Trailing 12 Months |
| `DbtS2NIPTM` |  | Previous Trailing 12 Months |
| `DbtS2NIA` |  | Latest Year |
| `DbtS2NIPY` |  | Previous Year |
| `DbtS2NIGr%PQ` |  | Q vs Previous Q Growth |
| `DbtS2NIGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtS2NIGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtS2NIGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtS2NIGr%A` |  | Growth Annual |
| `DbtS2NIGr%3Y` |  | Three Year Annualized Growth |
| `DbtS2NIGr%5Y` |  | Five Year Annualized Growth |
| `DbtS2NIGr%10Y` |  | Ten Year Annualized Growth |
| `DbtS2NIRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtS2NIRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtS2NIRegEstANN` |  | Ten Year Regression Estimate |
| `DbtS2NIRegEstTTM` |  | Five Year Regression Estimate |
| `DbtS2NIRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtS2NIRegGr%TTM` |  | Five Year Regression Growth |
| `DbtS2NI3YAvg` |  | Three Year Average |
| `DbtS2NI5YAvg` |  | Five Year Average |


### Depreciation And Amort to Gross Profit

D&A expenses relative to gross profit

| Factor | Params | Variant |
|--------|--------|---------|
| `DepAmort2GP()` | offset, type[, NAHandling] |  |
| `DepAmort2GPQ` |  | Latest Quarter |
| `DepAmort2GPPQ` |  | Previous Quarter |
| `DepAmort2GPPYQ` |  | Previous Quarter 1 Year Ago |
| `DepAmort2GPTTM` |  | Trailing 12 Months |
| `DepAmort2GPPTM` |  | Previous Trailing 12 Months |
| `DepAmort2GPA` |  | Latest Year |
| `DepAmort2GPPY` |  | Previous Year |
| `DepAmort2GPGr%PQ` |  | Q vs Previous Q Growth |
| `DepAmort2GPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DepAmort2GPGr%TTM` |  | Trailing Twelve Months Growth |
| `DepAmort2GPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DepAmort2GPGr%A` |  | Growth Annual |
| `DepAmort2GPGr%3Y` |  | Three Year Annualized Growth |
| `DepAmort2GPGr%5Y` |  | Five Year Annualized Growth |
| `DepAmort2GPGr%10Y` |  | Ten Year Annualized Growth |
| `DepAmort2GPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DepAmort2GPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DepAmort2GPRegEstANN` |  | Ten Year Regression Estimate |
| `DepAmort2GPRegEstTTM` |  | Five Year Regression Estimate |
| `DepAmort2GPRegGr%ANN` |  | Ten Year Regression Estimate |
| `DepAmort2GPRegGr%TTM` |  | Five Year Regression Growth |
| `DepAmort2GPPSQ` |  | Quarterly Per Share |
| `DepAmort2GPPSA` |  | Annual Per Share |
| `DepAmort2GP%SalesQ` |  | % of Quarterly Sales |
| `DepAmort2GP%SalesA` |  | % of Annual Sales |
| `DepAmort2GP%AssetsQ` |  | % of Quarterly Assets |
| `DepAmort2GP%AssetsA` |  | % of Annual Assets |
| `DepAmort2GP3YAvg` |  | Three Year Average |
| `DepAmort2GP5YAvg` |  | Five Year Average |


### Interest Coverage

Measure of ability to pay interest expenses.

| Factor | Params | Variant |
|--------|--------|---------|
| `IntCov()` | offset, type[, NAHandling] |  |
| `IntCovQ` |  | Latest Quarter |
| `IntCovPQ` |  | Previous Quarter |
| `IntCovPYQ` |  | Previous Quarter 1 Year Ago |
| `IntCovTTM` |  | Trailing 12 Months |
| `IntCovPTM` |  | Previous Trailing 12 Months |
| `IntCovA` |  | Latest Year |
| `IntCovPY` |  | Previous Year |
| `IntCovGr%PQ` |  | Q vs Previous Q Growth |
| `IntCovGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IntCovGr%TTM` |  | Trailing Twelve Months Growth |
| `IntCovGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IntCovGr%A` |  | Growth Annual |
| `IntCovGr%3Y` |  | Three Year Annualized Growth |
| `IntCovGr%5Y` |  | Five Year Annualized Growth |
| `IntCovGr%10Y` |  | Ten Year Annualized Growth |
| `IntCovRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IntCovRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IntCovRegEstANN` |  | Ten Year Regression Estimate |
| `IntCovRegEstTTM` |  | Five Year Regression Estimate |
| `IntCovRegGr%ANN` |  | Ten Year Regression Estimate |
| `IntCovRegGr%TTM` |  | Five Year Regression Growth |
| `IntCov3YAvg` |  | Three Year Average |
| `IntCov5YAvg` |  | Five Year Average |


### Long Term Debt to Total Assets

Long-term debt relative to total assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLT2Ast()` | offset, type[, NAHandling] |  |
| `DbtLT2AstQ` |  | Latest Quarter |
| `DbtLT2AstPQ` |  | Previous Quarter |
| `DbtLT2AstPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLT2AstTTM` |  | Trailing 12 Months |
| `DbtLT2AstPTM` |  | Previous Trailing 12 Months |
| `DbtLT2AstA` |  | Latest Year |
| `DbtLT2AstPY` |  | Previous Year |
| `DbtLT2AstGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLT2AstGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLT2AstGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLT2AstGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLT2AstGr%A` |  | Growth Annual |
| `DbtLT2AstGr%3Y` |  | Three Year Annualized Growth |
| `DbtLT2AstGr%5Y` |  | Five Year Annualized Growth |
| `DbtLT2AstGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLT2AstRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLT2AstRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLT2AstRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLT2AstRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLT2AstRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLT2AstRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLT2Ast3YAvg` |  | Three Year Average |
| `DbtLT2Ast5YAvg` |  | Five Year Average |


### Long Term Debt to Total Capital

Long-term debt relative to total capital.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLT2Cap()` | offset, type[, NAHandling] |  |
| `DbtLT2CapQ` |  | Latest Quarter |
| `DbtLT2CapPQ` |  | Previous Quarter |
| `DbtLT2CapPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLT2CapTTM` |  | Trailing 12 Months |
| `DbtLT2CapPTM` |  | Previous Trailing 12 Months |
| `DbtLT2CapA` |  | Latest Year |
| `DbtLT2CapPY` |  | Previous Year |
| `DbtLT2CapGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLT2CapGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLT2CapGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLT2CapGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLT2CapGr%A` |  | Growth Annual |
| `DbtLT2CapGr%3Y` |  | Three Year Annualized Growth |
| `DbtLT2CapGr%5Y` |  | Five Year Annualized Growth |
| `DbtLT2CapGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLT2CapRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLT2CapRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLT2CapRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLT2CapRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLT2CapRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLT2CapRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLT2Cap3YAvg` |  | Three Year Average |
| `DbtLT2Cap5YAvg` |  | Five Year Average |


### Long Term Debt to Total Equity

Long-term debt relative to common equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLT2Eq()` | offset, type[, NAHandling] |  |
| `DbtLT2EqQ` |  | Latest Quarter |
| `DbtLT2EqPQ` |  | Previous Quarter |
| `DbtLT2EqPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLT2EqTTM` |  | Trailing 12 Months |
| `DbtLT2EqPTM` |  | Previous Trailing 12 Months |
| `DbtLT2EqA` |  | Latest Year |
| `DbtLT2EqPY` |  | Previous Year |
| `DbtLT2EqGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLT2EqGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLT2EqGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLT2EqGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLT2EqGr%A` |  | Growth Annual |
| `DbtLT2EqGr%3Y` |  | Three Year Annualized Growth |
| `DbtLT2EqGr%5Y` |  | Five Year Annualized Growth |
| `DbtLT2EqGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLT2EqRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLT2EqRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLT2EqRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLT2EqRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLT2EqRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLT2EqRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLT2Eq3YAvg` |  | Three Year Average |
| `DbtLT2Eq5YAvg` |  | Five Year Average |


### Net Income to Cap Expenditures

Profit is reinvested in capital expenditures.

| Factor | Params | Variant |
|--------|--------|---------|
| `NI2CapEx()` | offset, type[, NAHandling] |  |
| `NI2CapExQ` |  | Latest Quarter |
| `NI2CapExPQ` |  | Previous Quarter |
| `NI2CapExPYQ` |  | Previous Quarter 1 Year Ago |
| `NI2CapExTTM` |  | Trailing 12 Months |
| `NI2CapExPTM` |  | Previous Trailing 12 Months |
| `NI2CapExA` |  | Latest Year |
| `NI2CapExPY` |  | Previous Year |
| `NI2CapExGr%PQ` |  | Q vs Previous Q Growth |
| `NI2CapExGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NI2CapExGr%TTM` |  | Trailing Twelve Months Growth |
| `NI2CapExGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NI2CapExGr%A` |  | Growth Annual |
| `NI2CapExGr%3Y` |  | Three Year Annualized Growth |
| `NI2CapExGr%5Y` |  | Five Year Annualized Growth |
| `NI2CapExGr%10Y` |  | Ten Year Annualized Growth |
| `NI2CapExRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NI2CapExRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NI2CapExRegEstANN` |  | Ten Year Regression Estimate |
| `NI2CapExRegEstTTM` |  | Five Year Regression Estimate |
| `NI2CapExRegGr%ANN` |  | Ten Year Regression Estimate |
| `NI2CapExRegGr%TTM` |  | Five Year Regression Growth |
| `NI2CapExPSQ` |  | Quarterly Per Share |
| `NI2CapExPSA` |  | Annual Per Share |
| `NI2CapEx%SalesQ` |  | % of Quarterly Sales |
| `NI2CapEx%SalesA` |  | % of Annual Sales |
| `NI2CapEx%AssetsQ` |  | % of Quarterly Assets |
| `NI2CapEx%AssetsA` |  | % of Annual Assets |
| `NI2CapEx3YAvg` |  | Three Year Average |
| `NI2CapEx5YAvg` |  | Five Year Average |


### Payout Ratio

Pividends paid relative to net income.

| Factor | Params | Variant |
|--------|--------|---------|
| `PayRatio()` | offset, type[, NAHandling] |  |
| `PayRatioQ` |  | Latest Quarter |
| `PayRatioPQ` |  | Previous Quarter |
| `PayRatioPYQ` |  | Previous Quarter 1 Year Ago |
| `PayRatioTTM` |  | Trailing 12 Months |
| `PayRatioPTM` |  | Previous Trailing 12 Months |
| `PayRatioA` |  | Latest Year |
| `PayRatioPY` |  | Previous Year |
| `PayRatioGr%PQ` |  | Q vs Previous Q Growth |
| `PayRatioGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PayRatioGr%TTM` |  | Trailing Twelve Months Growth |
| `PayRatioGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PayRatioGr%A` |  | Growth Annual |
| `PayRatioGr%3Y` |  | Three Year Annualized Growth |
| `PayRatioGr%5Y` |  | Five Year Annualized Growth |
| `PayRatioGr%10Y` |  | Ten Year Annualized Growth |
| `PayRatioRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PayRatioRSD%TTM` |  | Five Year Relative Standard Deviation |
| `PayRatioRegEstANN` |  | Ten Year Regression Estimate |
| `PayRatioRegEstTTM` |  | Five Year Regression Estimate |
| `PayRatioRegGr%ANN` |  | Ten Year Regression Estimate |
| `PayRatioRegGr%TTM` |  | Five Year Regression Growth |
| `PayRatio3YAvg` |  | Three Year Average |
| `PayRatio5YAvg` |  | Five Year Average |
| `PayRatio5Y` |  | 5 Years |


### Quick  Ratio

Immediate liquidity excluding inventory.

| Factor | Params | Variant |
|--------|--------|---------|
| `QuickRatio()` | offset, type[, NAHandling] |  |
| `QuickRatioQ` |  | Latest Quarter |
| `QuickRatioPQ` |  | Previous Quarter |
| `QuickRatioPYQ` |  | Previous Quarter 1 Year Ago |
| `QuickRatioTTM` |  | Trailing 12 Months |
| `QuickRatioPTM` |  | Previous Trailing 12 Months |
| `QuickRatioA` |  | Latest Year |
| `QuickRatioPY` |  | Previous Year |
| `QuickRatioGr%PQ` |  | Q vs Previous Q Growth |
| `QuickRatioGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `QuickRatioGr%TTM` |  | Trailing Twelve Months Growth |
| `QuickRatioGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `QuickRatioGr%A` |  | Growth Annual |
| `QuickRatioGr%3Y` |  | Three Year Annualized Growth |
| `QuickRatioGr%5Y` |  | Five Year Annualized Growth |
| `QuickRatioGr%10Y` |  | Ten Year Annualized Growth |
| `QuickRatioRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `QuickRatioRSD%TTM` |  | Five Year Relative Standard Deviation |
| `QuickRatioRegEstANN` |  | Ten Year Regression Estimate |
| `QuickRatioRegEstTTM` |  | Five Year Regression Estimate |
| `QuickRatioRegGr%ANN` |  | Ten Year Regression Estimate |
| `QuickRatioRegGr%TTM` |  | Five Year Regression Growth |
| `QuickRatio3YAvg` |  | Three Year Average |
| `QuickRatio5YAvg` |  | Five Year Average |


### Retention Rate

Percentage of earnings kept by the company for reinvestment rather than distributed as dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `Retn%()` | offset, type[, NAHandling] |  |
| `Retn%Q` |  | Latest Quarter |
| `Retn%PQ` |  | Previous Quarter |
| `Retn%PYQ` |  | Previous Quarter 1 Year Ago |
| `Retn%TTM` |  | Trailing 12 Months |
| `Retn%PTM` |  | Previous Trailing 12 Months |
| `Retn%A` |  | Latest Year |
| `Retn%PY` |  | Previous Year |
| `Retn%Gr%PQ` |  | Q vs Previous Q Growth |
| `Retn%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `Retn%Gr%TTM` |  | Trailing Twelve Months Growth |
| `Retn%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `Retn%Gr%A` |  | Growth Annual |
| `Retn%Gr%3Y` |  | Three Year Annualized Growth |
| `Retn%Gr%5Y` |  | Five Year Annualized Growth |
| `Retn%Gr%10Y` |  | Ten Year Annualized Growth |
| `Retn%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `Retn%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `Retn%RegEstANN` |  | Ten Year Regression Estimate |
| `Retn%RegEstTTM` |  | Five Year Regression Estimate |
| `Retn%RegGr%ANN` |  | Ten Year Regression Estimate |
| `Retn%RegGr%TTM` |  | Five Year Regression Growth |
| `Retn%3YAvg` |  | Three Year Average |
| `Retn%5YAvg` |  | Five Year Average |


### Total Debt To Total Assets

Total debt relative to total assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtTot2Ast()` | offset, type[, NAHandling] |  |
| `DbtTot2AstQ` |  | Latest Quarter |
| `DbtTot2AstPQ` |  | Previous Quarter |
| `DbtTot2AstPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtTot2AstTTM` |  | Trailing 12 Months |
| `DbtTot2AstPTM` |  | Previous Trailing 12 Months |
| `DbtTot2AstA` |  | Latest Year |
| `DbtTot2AstPY` |  | Previous Year |
| `DbtTot2AstGr%PQ` |  | Q vs Previous Q Growth |
| `DbtTot2AstGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtTot2AstGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtTot2AstGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtTot2AstGr%A` |  | Growth Annual |
| `DbtTot2AstGr%3Y` |  | Three Year Annualized Growth |
| `DbtTot2AstGr%5Y` |  | Five Year Annualized Growth |
| `DbtTot2AstGr%10Y` |  | Ten Year Annualized Growth |
| `DbtTot2AstRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtTot2AstRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtTot2AstRegEstANN` |  | Ten Year Regression Estimate |
| `DbtTot2AstRegEstTTM` |  | Five Year Regression Estimate |
| `DbtTot2AstRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtTot2AstRegGr%TTM` |  | Five Year Regression Growth |
| `DbtTot2Ast3YAvg` |  | Three Year Average |
| `DbtTot2Ast5YAvg` |  | Five Year Average |


### Total Debt to Total Capital

Total debt relative to total capital.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtTot2Cap()` | offset, type[, NAHandling] |  |
| `DbtTot2CapQ` |  | Latest Quarter |
| `DbtTot2CapPQ` |  | Previous Quarter |
| `DbtTot2CapPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtTot2CapTTM` |  | Trailing 12 Months |
| `DbtTot2CapPTM` |  | Previous Trailing 12 Months |
| `DbtTot2CapA` |  | Latest Year |
| `DbtTot2CapPY` |  | Previous Year |
| `DbtTot2CapGr%PQ` |  | Q vs Previous Q Growth |
| `DbtTot2CapGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtTot2CapGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtTot2CapGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtTot2CapGr%A` |  | Growth Annual |
| `DbtTot2CapGr%3Y` |  | Three Year Annualized Growth |
| `DbtTot2CapGr%5Y` |  | Five Year Annualized Growth |
| `DbtTot2CapGr%10Y` |  | Ten Year Annualized Growth |
| `DbtTot2CapRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtTot2CapRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtTot2CapRegEstANN` |  | Ten Year Regression Estimate |
| `DbtTot2CapRegEstTTM` |  | Five Year Regression Estimate |
| `DbtTot2CapRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtTot2CapRegGr%TTM` |  | Five Year Regression Growth |
| `DbtTot2Cap3YAvg` |  | Three Year Average |
| `DbtTot2Cap5YAvg` |  | Five Year Average |


### Total Debt to Total Equity

Total debt relative to common equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtTot2Eq()` | offset, type[, NAHandling] |  |
| `DbtTot2EqQ` |  | Latest Quarter |
| `DbtTot2EqPQ` |  | Previous Quarter |
| `DbtTot2EqPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtTot2EqTTM` |  | Trailing 12 Months |
| `DbtTot2EqPTM` |  | Previous Trailing 12 Months |
| `DbtTot2EqA` |  | Latest Year |
| `DbtTot2EqPY` |  | Previous Year |
| `DbtTot2EqGr%PQ` |  | Q vs Previous Q Growth |
| `DbtTot2EqGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtTot2EqGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtTot2EqGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtTot2EqGr%A` |  | Growth Annual |
| `DbtTot2EqGr%3Y` |  | Three Year Annualized Growth |
| `DbtTot2EqGr%5Y` |  | Five Year Annualized Growth |
| `DbtTot2EqGr%10Y` |  | Ten Year Annualized Growth |
| `DbtTot2EqRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtTot2EqRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtTot2EqRegEstANN` |  | Ten Year Regression Estimate |
| `DbtTot2EqRegEstTTM` |  | Five Year Regression Estimate |
| `DbtTot2EqRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtTot2EqRegGr%TTM` |  | Five Year Regression Growth |
| `DbtTot2Eq3YAvg` |  | Three Year Average |
| `DbtTot2Eq5YAvg` |  | Five Year Average |


### Working Capital To Price

Working Capital Per Share To Price Ratio, Annual

| Factor | Params | Variant |
|--------|--------|---------|
| `WCapPS2PrA` |  | Latest Year |
| `WCapPS2PrQ` |  | Latest Quarter |


## Other

Other ratios and statistics.

### Earnings Per Share (EPS) Stability

EPS Stability (standard deviation of the past 20 quarters)

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSStableQ` |  | Previous Quarter |


### Enterprise Value

Enterprise Value is an estimated measure of the total value of a corporation.

| Factor | Params | Variant |
|--------|--------|---------|
| `EV` |  |  |
| `EVPS` |  |  |


### Float

Float (millions).  This is the number of the common shares outstanding that are freely available for public trading.

NOTE:Data is sporadic prior to 2004 and defaults to number of shares when it cannot be calculated

| Factor | Params | Variant |
|--------|--------|---------|
| `Float` |  |  |
| `FloatPct` |  |  |


### Income Trend

Consecutive years of positive EPS

| Factor | Params | Variant |
|--------|--------|---------|
| `EPS#Positive` |  |  |
| `NoIncP4YN2Y` |  |  |
| `NoPosEBITDA5Y` |  | 5 Years |
| `NoPosEPS5Q` |  | 5 Quarters |


### Market Capitalization

Market Capitalization ($ millions) - for stocks and closed-end funds (CEFs)

| Factor | Params | Variant |
|--------|--------|---------|
| `MktCap` |  |  |


### Value of Return On Equity

Value of Return On Equity, TTM {ratio}

| Factor | Params | Variant |
|--------|--------|---------|
| `ValROETTM` |  | Trailing 12 Months |


### NAV Growth

NAV percent change 12 months

| Factor | Params | Variant |
|--------|--------|---------|
| `NAV%Chg12M` |  | 12 Months |
| `NAV%Chg1M` |  | 1 Month |
| `NAV%Chg3M` |  | 3 Months |
| `NAV%Chg6M` |  | 6 Months |


### Sustainable Growth

Growth Sustainable (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `SusGr%` |  | Trailing 12 Months |


## Advanced

Beneish M-Score, Piotroski F-Score, Alman Z-score.

### Beneish M-Score

Beneish M-Score finds companies that are associated with increased probability of manipulations. Companies with M-score of -1.89 or lower are safest, while -1.49 or higher are riskiest.

| Factor | Params | Variant |
|--------|--------|---------|
| `BeneishMScore` |  | Trailing 12 Months |
| `MScoreAQI` |  | Trailing 12 Months |
| `MScoreDEPAMI` |  | Trailing 12 Months |
| `MScoreDEPI` |  | Trailing 12 Months |
| `MScoreDSRI` |  | Trailing 12 Months |
| `MScoreGMI` |  | Trailing 12 Months |
| `MScoreLVGI` |  | Trailing 12 Months |
| `MScoreSGAI` |  | Trailing 12 Months |
| `MScoreSGI` |  | Trailing 12 Months |
| `MScoreTATA` |  | Trailing 12 Months |


### Piotroski F-Score

Piotroski F-Score assigns a score from 0 (more likely to go bankrupt) to 9 (strong financials) based on 9 PASS/FAIL tests

| Factor | Params | Variant |
|--------|--------|---------|
| `PiotFScore` |  | Trailing 12 Months |


### Altman Z-Score

Original z-score, recommended cutoff is 1.81 or higher

| Factor | Params | Variant |
|--------|--------|---------|
| `AltmanZOrig` |  | Trailing 12 Months |
| `AltmanZPriv` |  | Trailing 12 Months |
| `AltmanZNonManu` |  | Trailing 12 Months |


### Altman X Component

Working Capital to Assets

| Factor | Params | Variant |
|--------|--------|---------|
| `AltmanX1` |  | Trailing 12 Months |
| `AltmanX2` |  | Trailing 12 Months |
| `AltmanX3` |  | Trailing 12 Months |
| `AltmanX4` |  | Trailing 12 Months |
| `AltmanX4Rev` |  | Trailing 12 Months |
| `AltmanX5` |  | Trailing 12 Months |

