# Financials

Financial statement line items from filings (annual, quarterly or semiannual) and press releases. Figures are standardized by the data vendor.

## Income Statement

Lines from the (consolidated) statement of income.

### Amortization of Intangibles

Write down value of non-physical assets like copyrights, patents, and brands.

| Factor | Params | Variant |
|--------|--------|---------|
| `Amort()` | offset, type[, NAHandling] |  |
| `AmortQ` |  | Latest Quarter |
| `AmortPQ` |  | Previous Quarter |
| `AmortPYQ` |  | Previous Quarter 1 Year Ago |
| `AmortTTM` |  | Trailing 12 Months |
| `AmortPTM` |  | Previous Trailing 12 Months |
| `AmortA` |  | Latest Year |
| `AmortPY` |  | Previous Year |
| `AmortGr%PQ` |  | Q vs Previous Q Growth |
| `AmortGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AmortGr%TTM` |  | Trailing Twelve Months Growth |
| `AmortGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AmortGr%A` |  | Growth Annual |
| `AmortGr%3Y` |  | Three Year Annualized Growth |
| `AmortGr%5Y` |  | Five Year Annualized Growth |
| `AmortGr%10Y` |  | Ten Year Annualized Growth |
| `AmortRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AmortRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AmortRegEstANN` |  | Ten Year Regression Estimate |
| `AmortRegEstTTM` |  | Five Year Regression Estimate |
| `AmortRegGr%ANN` |  | Ten Year Regression Estimate |
| `AmortRegGr%TTM` |  | Five Year Regression Growth |
| `AmortPSQ` |  | Quarterly Per Share |
| `AmortPSA` |  | Annual Per Share |
| `Amort%SalesQ` |  | % of Quarterly Sales |
| `Amort%SalesA` |  | % of Annual Sales |
| `Amort%AssetsQ` |  | % of Quarterly Assets |
| `Amort%AssetsA` |  | % of Annual Assets |
| `Amort3YAvg` |  | Three Year Average |
| `Amort5YAvg` |  | Five Year Average |


### Cost of Goods Sold

Direct production expenses. CostG = Direct Materials + Direct Labor (excludes D&A).

| Factor | Params | Variant |
|--------|--------|---------|
| `CostG()` | offset, type[, NAHandling] |  |
| `CostGQ` |  | Latest Quarter |
| `CostGPQ` |  | Previous Quarter |
| `CostGPYQ` |  | Previous Quarter 1 Year Ago |
| `CostGTTM` |  | Trailing 12 Months |
| `CostGPTM` |  | Previous Trailing 12 Months |
| `CostGA` |  | Latest Year |
| `CostGPY` |  | Previous Year |
| `CostGGr%PQ` |  | Q vs Previous Q Growth |
| `CostGGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CostGGr%TTM` |  | Trailing Twelve Months Growth |
| `CostGGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CostGGr%A` |  | Growth Annual |
| `CostGGr%3Y` |  | Three Year Annualized Growth |
| `CostGGr%5Y` |  | Five Year Annualized Growth |
| `CostGGr%10Y` |  | Ten Year Annualized Growth |
| `CostGRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CostGRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CostGRegEstANN` |  | Ten Year Regression Estimate |
| `CostGRegEstTTM` |  | Five Year Regression Estimate |
| `CostGRegGr%ANN` |  | Ten Year Regression Estimate |
| `CostGRegGr%TTM` |  | Five Year Regression Growth |
| `CostGPSQ` |  | Quarterly Per Share |
| `CostGPSA` |  | Annual Per Share |
| `CostG%SalesQ` |  | % of Quarterly Sales |
| `CostG%SalesA` |  | % of Annual Sales |
| `CostG3YAvg` |  | Three Year Average |
| `CostG5YAvg` |  | Five Year Average |


### Cost of Goods Sold GAAP

Direct production expenses. CostG_GAAP = Direct Materials + Direct Labor + D&A.

| Factor | Params | Variant |
|--------|--------|---------|
| `CostG_GAAP()` | offset, type[, NAHandling] |  |
| `CostG_GAAPQ` |  | Latest Quarter |
| `CostG_GAAPPQ` |  | Previous Quarter |
| `CostG_GAAPPYQ` |  | Previous Quarter 1 Year Ago |
| `CostG_GAAPTTM` |  | Trailing 12 Months |
| `CostG_GAAPPTM` |  | Previous Trailing 12 Months |
| `CostG_GAAPA` |  | Latest Year |
| `CostG_GAAPPY` |  | Previous Year |
| `CostG_GAAPGr%PQ` |  | Q vs Previous Q Growth |
| `CostG_GAAPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CostG_GAAPGr%TTM` |  | Trailing Twelve Months Growth |
| `CostG_GAAPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CostG_GAAPGr%A` |  | Growth Annual |
| `CostG_GAAPGr%3Y` |  | Three Year Annualized Growth |
| `CostG_GAAPGr%5Y` |  | Five Year Annualized Growth |
| `CostG_GAAPGr%10Y` |  | Ten Year Annualized Growth |
| `CostG_GAAPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CostG_GAAPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CostG_GAAPRegEstANN` |  | Ten Year Regression Estimate |
| `CostG_GAAPRegEstTTM` |  | Five Year Regression Estimate |
| `CostG_GAAPRegGr%ANN` |  | Ten Year Regression Estimate |
| `CostG_GAAPRegGr%TTM` |  | Five Year Regression Growth |
| `CostG_GAAPPSQ` |  | Quarterly Per Share |
| `CostG_GAAPPSA` |  | Annual Per Share |
| `CostG_GAAP%SalesQ` |  | % of Quarterly Sales |
| `CostG_GAAP%SalesA` |  | % of Annual Sales |
| `CostG_GAAP3YAvg` |  | Three Year Average |
| `CostG_GAAP5YAvg` |  | Five Year Average |


### Depreciation and Amortization

The sum of D&A expenses as reported specifically on income statement.

| Factor | Params | Variant |
|--------|--------|---------|
| `DepAmort()` | offset, type[, NAHandling] |  |
| `DepAmortQ` |  | Latest Quarter |
| `DepAmortPQ` |  | Previous Quarter |
| `DepAmortPYQ` |  | Previous Quarter 1 Year Ago |
| `DepAmortTTM` |  | Trailing 12 Months |
| `DepAmortPTM` |  | Previous Trailing 12 Months |
| `DepAmortA` |  | Latest Year |
| `DepAmortPY` |  | Previous Year |
| `DepAmortGr%PQ` |  | Q vs Previous Q Growth |
| `DepAmortGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DepAmortGr%TTM` |  | Trailing Twelve Months Growth |
| `DepAmortGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DepAmortGr%A` |  | Growth Annual |
| `DepAmortGr%3Y` |  | Three Year Annualized Growth |
| `DepAmortGr%5Y` |  | Five Year Annualized Growth |
| `DepAmortGr%10Y` |  | Ten Year Annualized Growth |
| `DepAmortRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DepAmortRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DepAmortRegEstANN` |  | Ten Year Regression Estimate |
| `DepAmortRegEstTTM` |  | Five Year Regression Estimate |
| `DepAmortRegGr%ANN` |  | Ten Year Regression Estimate |
| `DepAmortRegGr%TTM` |  | Five Year Regression Growth |
| `DepAmortPSQ` |  | Quarterly Per Share |
| `DepAmortPSA` |  | Annual Per Share |
| `DepAmort%SalesQ` |  | % of Quarterly Sales |
| `DepAmort%SalesA` |  | % of Annual Sales |
| `DepAmort3YAvg` |  | Three Year Average |
| `DepAmort5YAvg` |  | Five Year Average |


### Earnings Before Interest and Taxes (EBIT)

Operating income including depreciation and amortization.

| Factor | Params | Variant |
|--------|--------|---------|
| `EBIT()` | offset, type[, NAHandling] |  |
| `EBITQ` |  | Latest Quarter |
| `EBITPQ` |  | Previous Quarter |
| `EBITPYQ` |  | Previous Quarter 1 Year Ago |
| `EBITTTM` |  | Trailing 12 Months |
| `EBITPTM` |  | Previous Trailing 12 Months |
| `EBITA` |  | Latest Year |
| `EBITPY` |  | Previous Year |
| `EBITGr%PQ` |  | Q vs Previous Q Growth |
| `EBITGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EBITGr%TTM` |  | Trailing Twelve Months Growth |
| `EBITGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EBITGr%A` |  | Growth Annual |
| `EBITGr%3Y` |  | Three Year Annualized Growth |
| `EBITGr%5Y` |  | Five Year Annualized Growth |
| `EBITGr%10Y` |  | Ten Year Annualized Growth |
| `EBITRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EBITRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EBITRegEstANN` |  | Ten Year Regression Estimate |
| `EBITRegEstTTM` |  | Five Year Regression Estimate |
| `EBITRegGr%ANN` |  | Ten Year Regression Estimate |
| `EBITRegGr%TTM` |  | Five Year Regression Growth |
| `EBITPSQ` |  | Quarterly Per Share |
| `EBITPSA` |  | Annual Per Share |
| `EBIT%SalesQ` |  | % of Quarterly Sales |
| `EBIT%SalesA` |  | % of Annual Sales |
| `EBIT3YAvg` |  | Three Year Average |
| `EBIT5YAvg` |  | Five Year Average |


### Earnings Before Interest, Taxes, Dep and Amort (EBITDA)

Operating income excluding non-cash expenses D&A.

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDA()` | offset, type[, NAHandling] |  |
| `EBITDAQ` |  | Latest Quarter |
| `EBITDAPQ` |  | Previous Quarter |
| `EBITDAPYQ` |  | Previous Quarter 1 Year Ago |
| `EBITDATTM` |  | Trailing 12 Months |
| `EBITDAPTM` |  | Previous Trailing 12 Months |
| `EBITDAA` |  | Latest Year |
| `EBITDAPY` |  | Previous Year |
| `EBITDAGr%PQ` |  | Q vs Previous Q Growth |
| `EBITDAGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EBITDAGr%TTM` |  | Trailing Twelve Months Growth |
| `EBITDAGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EBITDAGr%A` |  | Growth Annual |
| `EBITDAGr%3Y` |  | Three Year Annualized Growth |
| `EBITDAGr%5Y` |  | Five Year Annualized Growth |
| `EBITDAGr%10Y` |  | Ten Year Annualized Growth |
| `EBITDARSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EBITDARSD%TTM` |  | Five Year Relative Standard Deviation |
| `EBITDARegEstANN` |  | Ten Year Regression Estimate |
| `EBITDARegEstTTM` |  | Five Year Regression Estimate |
| `EBITDARegGr%ANN` |  | Ten Year Regression Estimate |
| `EBITDARegGr%TTM` |  | Five Year Regression Growth |
| `EBITDAPSQ` |  | Quarterly Per Share |
| `EBITDAPSA` |  | Annual Per Share |
| `EBITDA%SalesQ` |  | % of Quarterly Sales |
| `EBITDA%SalesA` |  | % of Annual Sales |
| `EBITDA3YAvg` |  | Three Year Average |
| `EBITDA5YAvg` |  | Five Year Average |


### Funds From Operations

Funds From Operations

| Factor | Params | Variant |
|--------|--------|---------|
| `FundsFromOp()` | offset, type[, NAHandling] |  |
| `FundsFromOpQ` |  | Latest Quarter |
| `FundsFromOpPQ` |  | Previous Quarter |
| `FundsFromOpPYQ` |  | Previous Quarter 1 Year Ago |
| `FundsFromOpTTM` |  | Trailing 12 Months |
| `FundsFromOpPTM` |  | Previous Trailing 12 Months |
| `FundsFromOpA` |  | Latest Year |
| `FundsFromOpPY` |  | Previous Year |
| `FundsFromOpGr%PQ` |  | Q vs Previous Q Growth |
| `FundsFromOpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `FundsFromOpGr%TTM` |  | Trailing Twelve Months Growth |
| `FundsFromOpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `FundsFromOpGr%A` |  | Growth Annual |
| `FundsFromOpGr%3Y` |  | Three Year Annualized Growth |
| `FundsFromOpGr%5Y` |  | Five Year Annualized Growth |
| `FundsFromOpGr%10Y` |  | Ten Year Annualized Growth |
| `FundsFromOpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `FundsFromOpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `FundsFromOpRegEstANN` |  | Ten Year Regression Estimate |
| `FundsFromOpRegEstTTM` |  | Five Year Regression Estimate |
| `FundsFromOpRegGr%ANN` |  | Ten Year Regression Estimate |
| `FundsFromOpRegGr%TTM` |  | Five Year Regression Growth |
| `FundsFromOpPSQ` |  | Quarterly Per Share |
| `FundsFromOpPSA` |  | Annual Per Share |
| `FundsFromOp%SalesQ` |  | % of Quarterly Sales |
| `FundsFromOp%SalesA` |  | % of Annual Sales |
| `FundsFromOp%AssetsQ` |  | % of Quarterly Assets |
| `FundsFromOp%AssetsA` |  | % of Annual Assets |
| `FundsFromOp3YAvg` |  | Three Year Average |
| `FundsFromOp5YAvg` |  | Five Year Average |


### Gross Profit

Profit after deducting production/service costs. GrossProfit = Sales - CostG (excludes D&A).

| Factor | Params | Variant |
|--------|--------|---------|
| `GrossProfit()` | offset, type[, NAHandling] |  |
| `GrossProfitQ` |  | Latest Quarter |
| `GrossProfitPQ` |  | Previous Quarter |
| `GrossProfitPYQ` |  | Previous Quarter 1 Year Ago |
| `GrossProfitTTM` |  | Trailing 12 Months |
| `GrossProfitPTM` |  | Previous Trailing 12 Months |
| `GrossProfitA` |  | Latest Year |
| `GrossProfitPY` |  | Previous Year |
| `GrossProfitGr%PQ` |  | Q vs Previous Q Growth |
| `GrossProfitGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GrossProfitGr%TTM` |  | Trailing Twelve Months Growth |
| `GrossProfitGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GrossProfitGr%A` |  | Growth Annual |
| `GrossProfitGr%3Y` |  | Three Year Annualized Growth |
| `GrossProfitGr%5Y` |  | Five Year Annualized Growth |
| `GrossProfitGr%10Y` |  | Ten Year Annualized Growth |
| `GrossProfitRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GrossProfitRSD%TTM` |  | Five Year Relative Standard Deviation |
| `GrossProfitRegEstANN` |  | Ten Year Regression Estimate |
| `GrossProfitRegEstTTM` |  | Five Year Regression Estimate |
| `GrossProfitRegGr%ANN` |  | Ten Year Regression Estimate |
| `GrossProfitRegGr%TTM` |  | Five Year Regression Growth |
| `GrossProfitPSQ` |  | Quarterly Per Share |
| `GrossProfitPSA` |  | Annual Per Share |
| `GrossProfit%SalesQ` |  | % of Quarterly Sales |
| `GrossProfit%SalesA` |  | % of Annual Sales |
| `GrossProfit%AssetsQ` |  | % of Quarterly Assets |
| `GrossProfit%AssetsA` |  | % of Annual Assets |
| `GrossProfit3YAvg` |  | Three Year Average |
| `GrossProfit5YAvg` |  | Five Year Average |


### Gross Profit GAAP

Profit after deducting production/service costs. GrossProfit_GAAP = Sales - CostG_GAAP (includes D&A).

| Factor | Params | Variant |
|--------|--------|---------|
| `GrossProfit_GAAP()` | offset, type[, NAHandling] |  |
| `GrossProfit_GAAPQ` |  | Latest Quarter |
| `GrossProfit_GAAPPQ` |  | Previous Quarter |
| `GrossProfit_GAAPPYQ` |  | Previous Quarter 1 Year Ago |
| `GrossProfit_GAAPTTM` |  | Trailing 12 Months |
| `GrossProfit_GAAPPTM` |  | Previous Trailing 12 Months |
| `GrossProfit_GAAPA` |  | Latest Year |
| `GrossProfit_GAAPPY` |  | Previous Year |
| `GrossProfit_GAAPGr%PQ` |  | Q vs Previous Q Growth |
| `GrossProfit_GAAPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GrossProfit_GAAPGr%TTM` |  | Trailing Twelve Months Growth |
| `GrossProfit_GAAPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GrossProfit_GAAPGr%A` |  | Growth Annual |
| `GrossProfit_GAAPGr%3Y` |  | Three Year Annualized Growth |
| `GrossProfit_GAAPGr%5Y` |  | Five Year Annualized Growth |
| `GrossProfit_GAAPGr%10Y` |  | Ten Year Annualized Growth |
| `GrossProfit_GAAPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GrossProfit_GAAPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `GrossProfit_GAAPRegEstANN` |  | Ten Year Regression Estimate |
| `GrossProfit_GAAPRegEstTTM` |  | Five Year Regression Estimate |
| `GrossProfit_GAAPRegGr%ANN` |  | Ten Year Regression Estimate |
| `GrossProfit_GAAPRegGr%TTM` |  | Five Year Regression Growth |
| `GrossProfit_GAAPPSQ` |  | Quarterly Per Share |
| `GrossProfit_GAAPPSA` |  | Annual Per Share |
| `GrossProfit_GAAP%SalesQ` |  | % of Quarterly Sales |
| `GrossProfit_GAAP%SalesA` |  | % of Annual Sales |
| `GrossProfit_GAAP%AssetsQ` |  | % of Quarterly Assets |
| `GrossProfit_GAAP%AssetsA` |  | % of Annual Assets |
| `GrossProfit_GAAP3YAvg` |  | Three Year Average |
| `GrossProfit_GAAP5YAvg` |  | Five Year Average |


### Impairment Charges

Represents the total charge against the carrying value of an asset to bring it to its fair value.

| Factor | Params | Variant |
|--------|--------|---------|
| `Impair()` | offset, type[, NAHandling] |  |
| `ImpairQ` |  | Latest Quarter |
| `ImpairPQ` |  | Previous Quarter |
| `ImpairPYQ` |  | Previous Quarter 1 Year Ago |
| `ImpairTTM` |  | Trailing 12 Months |
| `ImpairPTM` |  | Previous Trailing 12 Months |
| `ImpairA` |  | Latest Year |
| `ImpairPY` |  | Previous Year |
| `ImpairGr%PQ` |  | Q vs Previous Q Growth |
| `ImpairGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ImpairGr%TTM` |  | Trailing Twelve Months Growth |
| `ImpairGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ImpairGr%A` |  | Growth Annual |
| `ImpairGr%3Y` |  | Three Year Annualized Growth |
| `ImpairGr%5Y` |  | Five Year Annualized Growth |
| `ImpairGr%10Y` |  | Ten Year Annualized Growth |
| `ImpairRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ImpairRSD%TTM` |  | Five Year Relative Standard Deviation |
| `ImpairRegEstANN` |  | Ten Year Regression Estimate |
| `ImpairRegEstTTM` |  | Five Year Regression Estimate |
| `ImpairRegGr%ANN` |  | Ten Year Regression Estimate |
| `ImpairRegGr%TTM` |  | Five Year Regression Growth |
| `Impair3YAvg` |  | Three Year Average |
| `Impair5YAvg` |  | Five Year Average |


### Income After Taxes

Pre-tax income excluding extraordinary items less tax expense.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncAftTax()` | offset, type[, NAHandling] |  |
| `IncAftTaxQ` |  | Latest Quarter |
| `IncAftTaxPQ` |  | Previous Quarter |
| `IncAftTaxPYQ` |  | Previous Quarter 1 Year Ago |
| `IncAftTaxTTM` |  | Trailing 12 Months |
| `IncAftTaxPTM` |  | Previous Trailing 12 Months |
| `IncAftTaxA` |  | Latest Year |
| `IncAftTaxPY` |  | Previous Year |
| `IncAftTaxGr%PQ` |  | Q vs Previous Q Growth |
| `IncAftTaxGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncAftTaxGr%TTM` |  | Trailing Twelve Months Growth |
| `IncAftTaxGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncAftTaxGr%A` |  | Growth Annual |
| `IncAftTaxGr%3Y` |  | Three Year Annualized Growth |
| `IncAftTaxGr%5Y` |  | Five Year Annualized Growth |
| `IncAftTaxGr%10Y` |  | Ten Year Annualized Growth |
| `IncAftTaxRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncAftTaxRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncAftTaxRegEstANN` |  | Ten Year Regression Estimate |
| `IncAftTaxRegEstTTM` |  | Five Year Regression Estimate |
| `IncAftTaxRegGr%ANN` |  | Ten Year Regression Estimate |
| `IncAftTaxRegGr%TTM` |  | Five Year Regression Growth |
| `IncAftTaxPSQ` |  | Quarterly Per Share |
| `IncAftTaxPSA` |  | Annual Per Share |
| `IncAftTax%SalesQ` |  | % of Quarterly Sales |
| `IncAftTax%SalesA` |  | % of Annual Sales |
| `IncAftTax3YAvg` |  | Three Year Average |
| `IncAftTax5YAvg` |  | Five Year Average |


### Income Available to Common

Income before extraordinary items and discontinued operations less preferred dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `IAC()` | offset, type[, NAHandling] |  |
| `IACQ` |  | Latest Quarter |
| `IACPQ` |  | Previous Quarter |
| `IACPYQ` |  | Previous Quarter 1 Year Ago |
| `IACTTM` |  | Trailing 12 Months |
| `IACPTM` |  | Previous Trailing 12 Months |
| `IACA` |  | Latest Year |
| `IACPY` |  | Previous Year |
| `IACGr%PQ` |  | Q vs Previous Q Growth |
| `IACGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IACGr%TTM` |  | Trailing Twelve Months Growth |
| `IACGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IACGr%A` |  | Growth Annual |
| `IACGr%3Y` |  | Three Year Annualized Growth |
| `IACGr%5Y` |  | Five Year Annualized Growth |
| `IACGr%10Y` |  | Ten Year Annualized Growth |
| `IACRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IACRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IACRegEstANN` |  | Ten Year Regression Estimate |
| `IACRegEstTTM` |  | Five Year Regression Estimate |
| `IACRegGr%ANN` |  | Ten Year Regression Estimate |
| `IACRegGr%TTM` |  | Five Year Regression Growth |
| `IACPSQ` |  | Quarterly Per Share |
| `IACPSA` |  | Annual Per Share |
| `IAC%SalesQ` |  | % of Quarterly Sales |
| `IAC%SalesA` |  | % of Annual Sales |
| `IAC3YAvg` |  | Three Year Average |
| `IAC5YAvg` |  | Five Year Average |


### Income Before Taxes

Income Before Taxes includes all expenses except extraordinary and discontinued items.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncBTax()` | offset, type[, NAHandling] |  |
| `IncBTaxQ` |  | Latest Quarter |
| `IncBTaxPQ` |  | Previous Quarter |
| `IncBTaxPYQ` |  | Previous Quarter 1 Year Ago |
| `IncBTaxTTM` |  | Trailing 12 Months |
| `IncBTaxPTM` |  | Previous Trailing 12 Months |
| `IncBTaxA` |  | Latest Year |
| `IncBTaxPY` |  | Previous Year |
| `IncBTaxGr%PQ` |  | Q vs Previous Q Growth |
| `IncBTaxGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncBTaxGr%TTM` |  | Trailing Twelve Months Growth |
| `IncBTaxGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncBTaxGr%A` |  | Growth Annual |
| `IncBTaxGr%3Y` |  | Three Year Annualized Growth |
| `IncBTaxGr%5Y` |  | Five Year Annualized Growth |
| `IncBTaxGr%10Y` |  | Ten Year Annualized Growth |
| `IncBTaxRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncBTaxRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncBTaxRegEstANN` |  | Ten Year Regression Estimate |
| `IncBTaxRegEstTTM` |  | Five Year Regression Estimate |
| `IncBTaxRegGr%ANN` |  | Ten Year Regression Estimate |
| `IncBTaxRegGr%TTM` |  | Five Year Regression Growth |
| `IncBTaxPSQ` |  | Quarterly Per Share |
| `IncBTaxPSA` |  | Annual Per Share |
| `IncBTax%SalesQ` |  | % of Quarterly Sales |
| `IncBTax%SalesA` |  | % of Annual Sales |
| `IncBTax3YAvg` |  | Three Year Average |
| `IncBTax5YAvg` |  | Five Year Average |


### Income Before Xor Items Adj for Common

Net income available to common divided by fully diluted shares.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncBXorAdjCSE()` | offset, type[, NAHandling] |  |
| `IncBXorAdjCSEQ` |  | Latest Quarter |
| `IncBXorAdjCSEPQ` |  | Previous Quarter |
| `IncBXorAdjCSEPYQ` |  | Previous Quarter 1 Year Ago |
| `IncBXorAdjCSETTM` |  | Trailing 12 Months |
| `IncBXorAdjCSEPTM` |  | Previous Trailing 12 Months |
| `IncBXorAdjCSEA` |  | Latest Year |
| `IncBXorAdjCSEPY` |  | Previous Year |
| `IncBXorAdjCSEGr%PQ` |  | Q vs Previous Q Growth |
| `IncBXorAdjCSEGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncBXorAdjCSEGr%TTM` |  | Trailing Twelve Months Growth |
| `IncBXorAdjCSEGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncBXorAdjCSEGr%A` |  | Growth Annual |
| `IncBXorAdjCSEGr%3Y` |  | Three Year Annualized Growth |
| `IncBXorAdjCSEGr%5Y` |  | Five Year Annualized Growth |
| `IncBXorAdjCSEGr%10Y` |  | Ten Year Annualized Growth |
| `IncBXorAdjCSERSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncBXorAdjCSERSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncBXorAdjCSERegEstANN` |  | Ten Year Regression Estimate |
| `IncBXorAdjCSERegEstTTM` |  | Five Year Regression Estimate |
| `IncBXorAdjCSERegGr%ANN` |  | Ten Year Regression Estimate |
| `IncBXorAdjCSERegGr%TTM` |  | Five Year Regression Growth |
| `IncBXorAdjCSEPSQ` |  | Quarterly Per Share |
| `IncBXorAdjCSEPSA` |  | Annual Per Share |
| `IncBXorAdjCSE%SalesQ` |  | % of Quarterly Sales |
| `IncBXorAdjCSE%SalesA` |  | % of Annual Sales |
| `IncBXorAdjCSE3YAvg` |  | Three Year Average |
| `IncBXorAdjCSE5YAvg` |  | Five Year Average |


### Income Before Xor Items Avail for Common

Income before extraordinary/discontinued items minus preferred dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncBXorForCom()` | offset, type[, NAHandling] |  |
| `IncBXorForComQ` |  | Latest Quarter |
| `IncBXorForComPQ` |  | Previous Quarter |
| `IncBXorForComPYQ` |  | Previous Quarter 1 Year Ago |
| `IncBXorForComTTM` |  | Trailing 12 Months |
| `IncBXorForComPTM` |  | Previous Trailing 12 Months |
| `IncBXorForComA` |  | Latest Year |
| `IncBXorForComPY` |  | Previous Year |
| `IncBXorForComGr%PQ` |  | Q vs Previous Q Growth |
| `IncBXorForComGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncBXorForComGr%TTM` |  | Trailing Twelve Months Growth |
| `IncBXorForComGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncBXorForComGr%A` |  | Growth Annual |
| `IncBXorForComGr%3Y` |  | Three Year Annualized Growth |
| `IncBXorForComGr%5Y` |  | Five Year Annualized Growth |
| `IncBXorForComGr%10Y` |  | Ten Year Annualized Growth |
| `IncBXorForComRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncBXorForComRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncBXorForComRegEstANN` |  | Ten Year Regression Estimate |
| `IncBXorForComRegEstTTM` |  | Five Year Regression Estimate |
| `IncBXorForComRegGr%ANN` |  | Ten Year Regression Estimate |
| `IncBXorForComRegGr%TTM` |  | Five Year Regression Growth |
| `IncBXorForComPSQ` |  | Quarterly Per Share |
| `IncBXorForComPSA` |  | Annual Per Share |
| `IncBXorForCom%SalesQ` |  | % of Quarterly Sales |
| `IncBXorForCom%SalesA` |  | % of Annual Sales |
| `IncBXorForCom3YAvg` |  | Three Year Average |
| `IncBXorForCom5YAvg` |  | Five Year Average |


### Income Tax Expense

Net amount paid by the company during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `IncTaxExp()` | offset, type[, NAHandling] |  |
| `IncTaxExpQ` |  | Latest Quarter |
| `IncTaxExpPQ` |  | Previous Quarter |
| `IncTaxExpPYQ` |  | Previous Quarter 1 Year Ago |
| `IncTaxExpTTM` |  | Trailing 12 Months |
| `IncTaxExpPTM` |  | Previous Trailing 12 Months |
| `IncTaxExpA` |  | Latest Year |
| `IncTaxExpPY` |  | Previous Year |
| `IncTaxExpGr%PQ` |  | Q vs Previous Q Growth |
| `IncTaxExpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IncTaxExpGr%TTM` |  | Trailing Twelve Months Growth |
| `IncTaxExpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IncTaxExpGr%A` |  | Growth Annual |
| `IncTaxExpGr%3Y` |  | Three Year Annualized Growth |
| `IncTaxExpGr%5Y` |  | Five Year Annualized Growth |
| `IncTaxExpGr%10Y` |  | Ten Year Annualized Growth |
| `IncTaxExpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IncTaxExpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IncTaxExpRegEstANN` |  | Ten Year Regression Estimate |
| `IncTaxExpRegEstTTM` |  | Five Year Regression Estimate |
| `IncTaxExpRegGr%ANN` |  | Ten Year Regression Estimate |
| `IncTaxExpRegGr%TTM` |  | Five Year Regression Growth |
| `IncTaxExpPSQ` |  | Quarterly Per Share |
| `IncTaxExpPSA` |  | Annual Per Share |
| `IncTaxExp%SalesQ` |  | % of Quarterly Sales |
| `IncTaxExp%SalesA` |  | % of Annual Sales |
| `IncTaxExp3YAvg` |  | Three Year Average |
| `IncTaxExp5YAvg` |  | Five Year Average |


### Interest Expense

Amount paid to service all debt during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `IntExp()` | offset, type[, NAHandling] |  |
| `IntExpQ` |  | Latest Quarter |
| `IntExpPQ` |  | Previous Quarter |
| `IntExpPYQ` |  | Previous Quarter 1 Year Ago |
| `IntExpTTM` |  | Trailing 12 Months |
| `IntExpPTM` |  | Previous Trailing 12 Months |
| `IntExpA` |  | Latest Year |
| `IntExpPY` |  | Previous Year |
| `IntExpGr%PQ` |  | Q vs Previous Q Growth |
| `IntExpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IntExpGr%TTM` |  | Trailing Twelve Months Growth |
| `IntExpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IntExpGr%A` |  | Growth Annual |
| `IntExpGr%3Y` |  | Three Year Annualized Growth |
| `IntExpGr%5Y` |  | Five Year Annualized Growth |
| `IntExpGr%10Y` |  | Ten Year Annualized Growth |
| `IntExpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IntExpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IntExpRegEstANN` |  | Ten Year Regression Estimate |
| `IntExpRegEstTTM` |  | Five Year Regression Estimate |
| `IntExpRegGr%ANN` |  | Ten Year Regression Estimate |
| `IntExpRegGr%TTM` |  | Five Year Regression Growth |
| `IntExpPSQ` |  | Quarterly Per Share |
| `IntExpPSA` |  | Annual Per Share |
| `IntExp%SalesQ` |  | % of Quarterly Sales |
| `IntExp%SalesA` |  | % of Annual Sales |
| `IntExp3YAvg` |  | Three Year Average |
| `IntExp5YAvg` |  | Five Year Average |


### Interest Income

Amount earned from loans during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `IntInc()` | offset, type[, NAHandling] |  |
| `IntIncQ` |  | Latest Quarter |
| `IntIncPQ` |  | Previous Quarter |
| `IntIncPYQ` |  | Previous Quarter 1 Year Ago |
| `IntIncTTM` |  | Trailing 12 Months |
| `IntIncPTM` |  | Previous Trailing 12 Months |
| `IntIncA` |  | Latest Year |
| `IntIncPY` |  | Previous Year |
| `IntIncGr%PQ` |  | Q vs Previous Q Growth |
| `IntIncGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IntIncGr%TTM` |  | Trailing Twelve Months Growth |
| `IntIncGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IntIncGr%A` |  | Growth Annual |
| `IntIncGr%3Y` |  | Three Year Annualized Growth |
| `IntIncGr%5Y` |  | Five Year Annualized Growth |
| `IntIncGr%10Y` |  | Ten Year Annualized Growth |
| `IntIncRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IntIncRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IntIncRegEstANN` |  | Ten Year Regression Estimate |
| `IntIncRegEstTTM` |  | Five Year Regression Estimate |
| `IntIncRegGr%ANN` |  | Ten Year Regression Estimate |
| `IntIncRegGr%TTM` |  | Five Year Regression Growth |
| `IntIncPSQ` |  | Quarterly Per Share |
| `IntIncPSA` |  | Annual Per Share |
| `IntInc%SalesQ` |  | % of Quarterly Sales |
| `IntInc%SalesA` |  | % of Annual Sales |
| `IntInc3YAvg` |  | Three Year Average |
| `IntInc5YAvg` |  | Five Year Average |


### Net Income Before Xor

Income after all expenses including taxes and minority interest.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetIncBXor()` | offset, type[, NAHandling] |  |
| `NetIncBXorQ` |  | Latest Quarter |
| `NetIncBXorPQ` |  | Previous Quarter |
| `NetIncBXorPYQ` |  | Previous Quarter 1 Year Ago |
| `NetIncBXorTTM` |  | Trailing 12 Months |
| `NetIncBXorPTM` |  | Previous Trailing 12 Months |
| `NetIncBXorA` |  | Latest Year |
| `NetIncBXorPY` |  | Previous Year |
| `NetIncBXorGr%PQ` |  | Q vs Previous Q Growth |
| `NetIncBXorGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetIncBXorGr%TTM` |  | Trailing Twelve Months Growth |
| `NetIncBXorGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetIncBXorGr%A` |  | Growth Annual |
| `NetIncBXorGr%3Y` |  | Three Year Annualized Growth |
| `NetIncBXorGr%5Y` |  | Five Year Annualized Growth |
| `NetIncBXorGr%10Y` |  | Ten Year Annualized Growth |
| `NetIncBXorRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetIncBXorRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetIncBXorRegEstANN` |  | Ten Year Regression Estimate |
| `NetIncBXorRegEstTTM` |  | Five Year Regression Estimate |
| `NetIncBXorRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetIncBXorRegGr%TTM` |  | Five Year Regression Growth |
| `NetIncBXorPSQ` |  | Quarterly Per Share |
| `NetIncBXorPSA` |  | Annual Per Share |
| `NetIncBXor%SalesQ` |  | % of Quarterly Sales |
| `NetIncBXor%SalesA` |  | % of Annual Sales |
| `NetIncBXor3YAvg` |  | Three Year Average |
| `NetIncBXor5YAvg` |  | Five Year Average |


### Net Income Before Xor and Non-Control Interest

Total earnings excluding extraordinary items and minority interest.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetIncBXorNonC()` | offset, type[, NAHandling] |  |
| `NetIncBXorNonCQ` |  | Latest Quarter |
| `NetIncBXorNonCPQ` |  | Previous Quarter |
| `NetIncBXorNonCPYQ` |  | Previous Quarter 1 Year Ago |
| `NetIncBXorNonCTTM` |  | Trailing 12 Months |
| `NetIncBXorNonCPTM` |  | Previous Trailing 12 Months |
| `NetIncBXorNonCA` |  | Latest Year |
| `NetIncBXorNonCPY` |  | Previous Year |
| `NetIncBXorNonCGr%PQ` |  | Q vs Previous Q Growth |
| `NetIncBXorNonCGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetIncBXorNonCGr%TTM` |  | Trailing Twelve Months Growth |
| `NetIncBXorNonCGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetIncBXorNonCGr%A` |  | Growth Annual |
| `NetIncBXorNonCGr%3Y` |  | Three Year Annualized Growth |
| `NetIncBXorNonCGr%5Y` |  | Five Year Annualized Growth |
| `NetIncBXorNonCGr%10Y` |  | Ten Year Annualized Growth |
| `NetIncBXorNonCRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetIncBXorNonCRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetIncBXorNonCRegEstANN` |  | Ten Year Regression Estimate |
| `NetIncBXorNonCRegEstTTM` |  | Five Year Regression Estimate |
| `NetIncBXorNonCRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetIncBXorNonCRegGr%TTM` |  | Five Year Regression Growth |
| `NetIncBXorNonCPSQ` |  | Quarterly Per Share |
| `NetIncBXorNonCPSA` |  | Annual Per Share |
| `NetIncBXorNonC%SalesQ` |  | % of Quarterly Sales |
| `NetIncBXorNonC%SalesA` |  | % of Annual Sales |
| `NetIncBXorNonC3YAvg` |  | Three Year Average |
| `NetIncBXorNonC5YAvg` |  | Five Year Average |


### Non-Operating Expenses

Net result from secondary activities unrelated to core business.

| Factor | Params | Variant |
|--------|--------|---------|
| `ExpNonOp()` | offset, type[, NAHandling] |  |
| `ExpNonOpQ` |  | Latest Quarter |
| `ExpNonOpPQ` |  | Previous Quarter |
| `ExpNonOpPYQ` |  | Previous Quarter 1 Year Ago |
| `ExpNonOpTTM` |  | Trailing 12 Months |
| `ExpNonOpPTM` |  | Previous Trailing 12 Months |
| `ExpNonOpA` |  | Latest Year |
| `ExpNonOpPY` |  | Previous Year |
| `ExpNonOpGr%PQ` |  | Q vs Previous Q Growth |
| `ExpNonOpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ExpNonOpGr%TTM` |  | Trailing Twelve Months Growth |
| `ExpNonOpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ExpNonOpGr%A` |  | Growth Annual |
| `ExpNonOpGr%3Y` |  | Three Year Annualized Growth |
| `ExpNonOpGr%5Y` |  | Five Year Annualized Growth |
| `ExpNonOpGr%10Y` |  | Ten Year Annualized Growth |
| `ExpNonOpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ExpNonOpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `ExpNonOpRegEstANN` |  | Ten Year Regression Estimate |
| `ExpNonOpRegEstTTM` |  | Five Year Regression Estimate |
| `ExpNonOpRegGr%ANN` |  | Ten Year Regression Estimate |
| `ExpNonOpRegGr%TTM` |  | Five Year Regression Growth |
| `ExpNonOpPSQ` |  | Quarterly Per Share |
| `ExpNonOpPSA` |  | Annual Per Share |
| `ExpNonOp%SalesQ` |  | % of Quarterly Sales |
| `ExpNonOp%SalesA` |  | % of Annual Sales |
| `ExpNonOp3YAvg` |  | Three Year Average |
| `ExpNonOp5YAvg` |  | Five Year Average |


### Operating Income

Revenues minus cost of goods sold, SG&A, and depreciation/amortization.

| Factor | Params | Variant |
|--------|--------|---------|
| `OpInc()` | offset, type[, NAHandling] |  |
| `OpIncQ` |  | Latest Quarter |
| `OpIncPQ` |  | Previous Quarter |
| `OpIncPYQ` |  | Previous Quarter 1 Year Ago |
| `OpIncTTM` |  | Trailing 12 Months |
| `OpIncPTM` |  | Previous Trailing 12 Months |
| `OpIncA` |  | Latest Year |
| `OpIncPY` |  | Previous Year |
| `OpIncGr%PQ` |  | Q vs Previous Q Growth |
| `OpIncGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OpIncGr%TTM` |  | Trailing Twelve Months Growth |
| `OpIncGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OpIncGr%A` |  | Growth Annual |
| `OpIncGr%3Y` |  | Three Year Annualized Growth |
| `OpIncGr%5Y` |  | Five Year Annualized Growth |
| `OpIncGr%10Y` |  | Ten Year Annualized Growth |
| `OpIncRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OpIncRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OpIncRegEstANN` |  | Ten Year Regression Estimate |
| `OpIncRegEstTTM` |  | Five Year Regression Estimate |
| `OpIncRegGr%ANN` |  | Ten Year Regression Estimate |
| `OpIncRegGr%TTM` |  | Five Year Regression Growth |
| `OpIncPSQ` |  | Quarterly Per Share |
| `OpIncPSA` |  | Annual Per Share |
| `OpInc%SalesQ` |  | % of Quarterly Sales |
| `OpInc%SalesA` |  | % of Annual Sales |
| `OpInc3YAvg` |  | Three Year Average |
| `OpInc5YAvg` |  | Five Year Average |


### Operating Income After Depreciation

Revenues minus COGS, SG&A, and depreciation/amortization. Identical to Operating Income.

| Factor | Params | Variant |
|--------|--------|---------|
| `OpIncAftDepr()` | offset, type[, NAHandling] |  |
| `OpIncAftDeprQ` |  | Latest Quarter |
| `OpIncAftDeprPQ` |  | Previous Quarter |
| `OpIncAftDeprPYQ` |  | Previous Quarter 1 Year Ago |
| `OpIncAftDeprTTM` |  | Trailing 12 Months |
| `OpIncAftDeprPTM` |  | Previous Trailing 12 Months |
| `OpIncAftDeprA` |  | Latest Year |
| `OpIncAftDeprPY` |  | Previous Year |
| `OpIncAftDeprGr%PQ` |  | Q vs Previous Q Growth |
| `OpIncAftDeprGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OpIncAftDeprGr%TTM` |  | Trailing Twelve Months Growth |
| `OpIncAftDeprGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OpIncAftDeprGr%A` |  | Growth Annual |
| `OpIncAftDeprGr%3Y` |  | Three Year Annualized Growth |
| `OpIncAftDeprGr%5Y` |  | Five Year Annualized Growth |
| `OpIncAftDeprGr%10Y` |  | Ten Year Annualized Growth |
| `OpIncAftDeprRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OpIncAftDeprRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OpIncAftDeprRegEstANN` |  | Ten Year Regression Estimate |
| `OpIncAftDeprRegEstTTM` |  | Five Year Regression Estimate |
| `OpIncAftDeprRegGr%ANN` |  | Ten Year Regression Estimate |
| `OpIncAftDeprRegGr%TTM` |  | Five Year Regression Growth |
| `OpIncAftDeprPSQ` |  | Quarterly Per Share |
| `OpIncAftDeprPSA` |  | Annual Per Share |
| `OpIncAftDepr%SalesQ` |  | % of Quarterly Sales |
| `OpIncAftDepr%SalesA` |  | % of Annual Sales |
| `OpIncAftDepr3YAvg` |  | Three Year Average |
| `OpIncAftDepr5YAvg` |  | Five Year Average |


### Operating Income Before Depreciation

Revenues minus COGS and SG&A.

| Factor | Params | Variant |
|--------|--------|---------|
| `OpIncBDepr()` | offset, type[, NAHandling] |  |
| `OpIncBDeprQ` |  | Latest Quarter |
| `OpIncBDeprPQ` |  | Previous Quarter |
| `OpIncBDeprPYQ` |  | Previous Quarter 1 Year Ago |
| `OpIncBDeprTTM` |  | Trailing 12 Months |
| `OpIncBDeprPTM` |  | Previous Trailing 12 Months |
| `OpIncBDeprA` |  | Latest Year |
| `OpIncBDeprPY` |  | Previous Year |
| `OpIncBDeprGr%PQ` |  | Q vs Previous Q Growth |
| `OpIncBDeprGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OpIncBDeprGr%TTM` |  | Trailing Twelve Months Growth |
| `OpIncBDeprGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OpIncBDeprGr%A` |  | Growth Annual |
| `OpIncBDeprGr%3Y` |  | Three Year Annualized Growth |
| `OpIncBDeprGr%5Y` |  | Five Year Annualized Growth |
| `OpIncBDeprGr%10Y` |  | Ten Year Annualized Growth |
| `OpIncBDeprRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OpIncBDeprRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OpIncBDeprRegEstANN` |  | Ten Year Regression Estimate |
| `OpIncBDeprRegEstTTM` |  | Five Year Regression Estimate |
| `OpIncBDeprRegGr%ANN` |  | Ten Year Regression Estimate |
| `OpIncBDeprRegGr%TTM` |  | Five Year Regression Growth |
| `OpIncBDeprPSQ` |  | Quarterly Per Share |
| `OpIncBDeprPSA` |  | Annual Per Share |
| `OpIncBDepr%SalesQ` |  | % of Quarterly Sales |
| `OpIncBDepr%SalesA` |  | % of Annual Sales |
| `OpIncBDepr3YAvg` |  | Three Year Average |
| `OpIncBDepr5YAvg` |  | Five Year Average |


### Preferred Dividends Paid, Total

Total amount paid to preferred shareholders across all preferred share issues during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `PfdDiv()` | offset, type[, NAHandling] |  |
| `PfdDivQ` |  | Latest Quarter |
| `PfdDivPQ` |  | Previous Quarter |
| `PfdDivPYQ` |  | Previous Quarter 1 Year Ago |
| `PfdDivTTM` |  | Trailing 12 Months |
| `PfdDivPTM` |  | Previous Trailing 12 Months |
| `PfdDivA` |  | Latest Year |
| `PfdDivPY` |  | Previous Year |
| `PfdDivGr%PQ` |  | Q vs Previous Q Growth |
| `PfdDivGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PfdDivGr%TTM` |  | Trailing Twelve Months Growth |
| `PfdDivGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PfdDivGr%A` |  | Growth Annual |
| `PfdDivGr%3Y` |  | Three Year Annualized Growth |
| `PfdDivGr%5Y` |  | Five Year Annualized Growth |
| `PfdDivGr%10Y` |  | Ten Year Annualized Growth |
| `PfdDivRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PfdDivRSD%TTM` |  | Five Year Relative Standard Deviation |
| `PfdDivRegEstANN` |  | Ten Year Regression Estimate |
| `PfdDivRegEstTTM` |  | Five Year Regression Estimate |
| `PfdDivRegGr%ANN` |  | Ten Year Regression Estimate |
| `PfdDivRegGr%TTM` |  | Five Year Regression Growth |
| `PfdDivPSQ` |  | Quarterly Per Share |
| `PfdDivPSA` |  | Annual Per Share |
| `PfdDiv%SalesQ` |  | % of Quarterly Sales |
| `PfdDiv%SalesA` |  | % of Annual Sales |
| `PfdDiv%AssetsQ` |  | % of Quarterly Assets |
| `PfdDiv%AssetsA` |  | % of Annual Assets |
| `PfdDiv3YAvg` |  | Three Year Average |
| `PfdDiv5YAvg` |  | Five Year Average |


### Research and Development Expense

Spending on future products/services during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `RandD()` | offset, type[, NAHandling] |  |
| `RandDQ` |  | Latest Quarter |
| `RandDPQ` |  | Previous Quarter |
| `RandDPYQ` |  | Previous Quarter 1 Year Ago |
| `RandDTTM` |  | Trailing 12 Months |
| `RandDPTM` |  | Previous Trailing 12 Months |
| `RandDA` |  | Latest Year |
| `RandDPY` |  | Previous Year |
| `RandDGr%PQ` |  | Q vs Previous Q Growth |
| `RandDGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `RandDGr%TTM` |  | Trailing Twelve Months Growth |
| `RandDGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `RandDGr%A` |  | Growth Annual |
| `RandDGr%3Y` |  | Three Year Annualized Growth |
| `RandDGr%5Y` |  | Five Year Annualized Growth |
| `RandDGr%10Y` |  | Ten Year Annualized Growth |
| `RandDRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `RandDRSD%TTM` |  | Five Year Relative Standard Deviation |
| `RandDRegEstANN` |  | Ten Year Regression Estimate |
| `RandDRegEstTTM` |  | Five Year Regression Estimate |
| `RandDRegGr%ANN` |  | Ten Year Regression Estimate |
| `RandDRegGr%TTM` |  | Five Year Regression Growth |
| `RandDPSQ` |  | Quarterly Per Share |
| `RandDPSA` |  | Annual Per Share |
| `RandD%SalesQ` |  | % of Quarterly Sales |
| `RandD%SalesA` |  | % of Annual Sales |
| `RandD%AssetsQ` |  | % of Quarterly Assets |
| `RandD%AssetsA` |  | % of Annual Assets |
| `RandD3YAvg` |  | Three Year Average |
| `RandD5YAvg` |  | Five Year Average |


### Sales (International)

Represents sales generated from operations in foreign countries. Export sales are not included. Annual values only.

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesIntl()` | offset, type[, NAHandling] |  |
| `SalesIntlA` |  | Latest Year |
| `SalesIntlPY` |  | Previous Year |
| `SalesIntlGr%A` |  | Growth Annual |
| `SalesIntlGr%3Y` |  | Three Year Annualized Growth |
| `SalesIntlGr%5Y` |  | Five Year Annualized Growth |
| `SalesIntlGr%10Y` |  | Ten Year Annualized Growth |
| `SalesIntl3YAvg` |  | Three Year Average |
| `SalesIntl5YAvg` |  | Five Year Average |


### Sales (Revenues)

Total value of goods/services sold in a period.

| Factor | Params | Variant |
|--------|--------|---------|
| `Sales()` | offset, type[, NAHandling] |  |
| `SalesQ` |  | Latest Quarter |
| `SalesPQ` |  | Previous Quarter |
| `SalesPYQ` |  | Previous Quarter 1 Year Ago |
| `SalesTTM` |  | Trailing 12 Months |
| `SalesPTM` |  | Previous Trailing 12 Months |
| `SalesA` |  | Latest Year |
| `SalesPY` |  | Previous Year |
| `SalesGr%PQ` |  | Q vs Previous Q Growth |
| `SalesGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SalesGr%TTM` |  | Trailing Twelve Months Growth |
| `SalesGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SalesGr%A` |  | Growth Annual |
| `SalesGr%3Y` |  | Three Year Annualized Growth |
| `SalesGr%5Y` |  | Five Year Annualized Growth |
| `SalesGr%10Y` |  | Ten Year Annualized Growth |
| `SalesRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SalesRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SalesRegEstANN` |  | Ten Year Regression Estimate |
| `SalesRegEstTTM` |  | Five Year Regression Estimate |
| `SalesRegGr%ANN` |  | Ten Year Regression Estimate |
| `SalesRegGr%TTM` |  | Five Year Regression Growth |
| `SalesPSQ` |  | Quarterly Per Share |
| `SalesPSA` |  | Annual Per Share |
| `Sales%AssetsQ` |  | % of Quarterly Assets |
| `Sales%AssetsA` |  | % of Annual Assets |
| `Sales3YAvg` |  | Three Year Average |
| `Sales5YAvg` |  | Five Year Average |


### Sales, General and Admin Exp

Expenses include all general/administrative costs plus direct/indirect selling expenses - excludes R&D expenses.

| Factor | Params | Variant |
|--------|--------|---------|
| `SGandA()` | offset, type[, NAHandling] |  |
| `SGandAQ` |  | Latest Quarter |
| `SGandAPQ` |  | Previous Quarter |
| `SGandAPYQ` |  | Previous Quarter 1 Year Ago |
| `SGandATTM` |  | Trailing 12 Months |
| `SGandAPTM` |  | Previous Trailing 12 Months |
| `SGandAA` |  | Latest Year |
| `SGandAPY` |  | Previous Year |
| `SGandAGr%PQ` |  | Q vs Previous Q Growth |
| `SGandAGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SGandAGr%TTM` |  | Trailing Twelve Months Growth |
| `SGandAGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SGandAGr%A` |  | Growth Annual |
| `SGandAGr%3Y` |  | Three Year Annualized Growth |
| `SGandAGr%5Y` |  | Five Year Annualized Growth |
| `SGandAGr%10Y` |  | Ten Year Annualized Growth |
| `SGandARSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SGandARSD%TTM` |  | Five Year Relative Standard Deviation |
| `SGandARegEstANN` |  | Ten Year Regression Estimate |
| `SGandARegEstTTM` |  | Five Year Regression Estimate |
| `SGandARegGr%ANN` |  | Ten Year Regression Estimate |
| `SGandARegGr%TTM` |  | Five Year Regression Growth |
| `SGandAPSQ` |  | Quarterly Per Share |
| `SGandAPSA` |  | Annual Per Share |
| `SGandA%SalesQ` |  | % of Quarterly Sales |
| `SGandA%SalesA` |  | % of Annual Sales |
| `SGandA%AssetsQ` |  | % of Quarterly Assets |
| `SGandA%AssetsA` |  | % of Annual Assets |
| `SGandA3YAvg` |  | Three Year Average |
| `SGandA5YAvg` |  | Five Year Average |


### Sales, General and Admin Exp GAAP

Expenses include all general/administrative costs plus direct/indirect selling expenses - includes R&D expenses.

| Factor | Params | Variant |
|--------|--------|---------|
| `SGandA_GAAP()` | offset, type[, NAHandling] |  |
| `SGandA_GAAPQ` |  | Latest Quarter |
| `SGandA_GAAPPQ` |  | Previous Quarter |
| `SGandA_GAAPPYQ` |  | Previous Quarter 1 Year Ago |
| `SGandA_GAAPTTM` |  | Trailing 12 Months |
| `SGandA_GAAPPTM` |  | Previous Trailing 12 Months |
| `SGandA_GAAPA` |  | Latest Year |
| `SGandA_GAAPPY` |  | Previous Year |
| `SGandA_GAAPGr%PQ` |  | Q vs Previous Q Growth |
| `SGandA_GAAPGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SGandA_GAAPGr%TTM` |  | Trailing Twelve Months Growth |
| `SGandA_GAAPGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SGandA_GAAPGr%A` |  | Growth Annual |
| `SGandA_GAAPGr%3Y` |  | Three Year Annualized Growth |
| `SGandA_GAAPGr%5Y` |  | Five Year Annualized Growth |
| `SGandA_GAAPGr%10Y` |  | Ten Year Annualized Growth |
| `SGandA_GAAPRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SGandA_GAAPRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SGandA_GAAPRegEstANN` |  | Ten Year Regression Estimate |
| `SGandA_GAAPRegEstTTM` |  | Five Year Regression Estimate |
| `SGandA_GAAPRegGr%ANN` |  | Ten Year Regression Estimate |
| `SGandA_GAAPRegGr%TTM` |  | Five Year Regression Growth |
| `SGandA_GAAPPSQ` |  | Quarterly Per Share |
| `SGandA_GAAPPSA` |  | Annual Per Share |
| `SGandA_GAAP%SalesQ` |  | % of Quarterly Sales |
| `SGandA_GAAP%SalesA` |  | % of Annual Sales |
| `SGandA_GAAP%AssetsQ` |  | % of Quarterly Assets |
| `SGandA_GAAP%AssetsA` |  | % of Annual Assets |
| `SGandA_GAAP3YAvg` |  | Three Year Average |
| `SGandA_GAAP5YAvg` |  | Five Year Average |


### Special Items

Total pre-tax non-recurring items.

| Factor | Params | Variant |
|--------|--------|---------|
| `SpcItems()` | offset, type[, NAHandling] |  |
| `SpcItemsQ` |  | Latest Quarter |
| `SpcItemsPQ` |  | Previous Quarter |
| `SpcItemsPYQ` |  | Previous Quarter 1 Year Ago |
| `SpcItemsTTM` |  | Trailing 12 Months |
| `SpcItemsPTM` |  | Previous Trailing 12 Months |
| `SpcItemsA` |  | Latest Year |
| `SpcItemsPY` |  | Previous Year |
| `SpcItemsGr%PQ` |  | Q vs Previous Q Growth |
| `SpcItemsGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SpcItemsGr%TTM` |  | Trailing Twelve Months Growth |
| `SpcItemsGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SpcItemsGr%A` |  | Growth Annual |
| `SpcItemsGr%3Y` |  | Three Year Annualized Growth |
| `SpcItemsGr%5Y` |  | Five Year Annualized Growth |
| `SpcItemsGr%10Y` |  | Ten Year Annualized Growth |
| `SpcItemsRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SpcItemsRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SpcItemsRegEstANN` |  | Ten Year Regression Estimate |
| `SpcItemsRegEstTTM` |  | Five Year Regression Estimate |
| `SpcItemsRegGr%ANN` |  | Ten Year Regression Estimate |
| `SpcItemsRegGr%TTM` |  | Five Year Regression Growth |
| `SpcItemsPSQ` |  | Quarterly Per Share |
| `SpcItemsPSA` |  | Annual Per Share |
| `SpcItems%SalesQ` |  | % of Quarterly Sales |
| `SpcItems%SalesA` |  | % of Annual Sales |
| `SpcItems%AssetsQ` |  | % of Quarterly Assets |
| `SpcItems%AssetsA` |  | % of Annual Assets |
| `SpcItems3YAvg` |  | Three Year Average |
| `SpcItems5YAvg` |  | Five Year Average |


### Stock Option Compensation Expense

Income statement SBC. Data begins around 2003, with full annual coverage starting in 2008, and interim in 2017

| Factor | Params | Variant |
|--------|--------|---------|
| `StkOptExp()` | offset, type[, NAHandling] |  |
| `StkOptExpQ` |  | Latest Quarter |
| `StkOptExpPQ` |  | Previous Quarter |
| `StkOptExpPYQ` |  | Previous Quarter 1 Year Ago |
| `StkOptExpTTM` |  | Trailing 12 Months |
| `StkOptExpPTM` |  | Previous Trailing 12 Months |
| `StkOptExpA` |  | Latest Year |
| `StkOptExpPY` |  | Previous Year |
| `StkOptExpGr%PQ` |  | Q vs Previous Q Growth |
| `StkOptExpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `StkOptExpGr%TTM` |  | Trailing Twelve Months Growth |
| `StkOptExpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `StkOptExpGr%A` |  | Growth Annual |
| `StkOptExpGr%3Y` |  | Three Year Annualized Growth |
| `StkOptExpGr%5Y` |  | Five Year Annualized Growth |
| `StkOptExpGr%10Y` |  | Ten Year Annualized Growth |
| `StkOptExpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `StkOptExpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `StkOptExpRegEstANN` |  | Ten Year Regression Estimate |
| `StkOptExpRegEstTTM` |  | Five Year Regression Estimate |
| `StkOptExpRegGr%ANN` |  | Ten Year Regression Estimate |
| `StkOptExpRegGr%TTM` |  | Five Year Regression Growth |
| `StkOptExpPSQ` |  | Quarterly Per Share |
| `StkOptExpPSA` |  | Annual Per Share |
| `StkOptExp%SalesQ` |  | % of Quarterly Sales |
| `StkOptExp%SalesA` |  | % of Annual Sales |
| `StkOptExp3YAvg` |  | Three Year Average |
| `StkOptExp5YAvg` |  | Five Year Average |


### Tax Rate

Tax expense as percentage of pre-tax income.

| Factor | Params | Variant |
|--------|--------|---------|
| `TxRate%()` | offset, type[, NAHandling] |  |
| `TxRate%Q` |  | Latest Quarter |
| `TxRate%PQ` |  | Previous Quarter |
| `TxRate%PYQ` |  | Previous Quarter 1 Year Ago |
| `TxRate%TTM` |  | Trailing 12 Months |
| `TxRate%PTM` |  | Previous Trailing 12 Months |
| `TxRate%A` |  | Latest Year |
| `TxRate%PY` |  | Previous Year |
| `TxRate%Gr%PQ` |  | Q vs Previous Q Growth |
| `TxRate%Gr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TxRate%Gr%TTM` |  | Trailing Twelve Months Growth |
| `TxRate%Gr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TxRate%Gr%A` |  | Growth Annual |
| `TxRate%Gr%3Y` |  | Three Year Annualized Growth |
| `TxRate%Gr%5Y` |  | Five Year Annualized Growth |
| `TxRate%Gr%10Y` |  | Ten Year Annualized Growth |
| `TxRate%RSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TxRate%RSD%TTM` |  | Five Year Relative Standard Deviation |
| `TxRate%RegEstANN` |  | Ten Year Regression Estimate |
| `TxRate%RegEstTTM` |  | Five Year Regression Estimate |
| `TxRate%RegGr%ANN` |  | Ten Year Regression Estimate |
| `TxRate%RegGr%TTM` |  | Five Year Regression Growth |
| `TxRate%3YAvg` |  | Three Year Average |
| `TxRate%5YAvg` |  | Five Year Average |


## Balance Sheet

Lines from the (consolidated) balance sheet.

### Assets-Current

Owned items that are identified by the company as being collectible or liquid enough to be disposed of within the next 12 months.

#### Accounts Receivables

Amounts due to the company within 12 months, typically from credit sales.

| Factor | Params | Variant |
|--------|--------|---------|
| `Recvbl()` | offset, type[, NAHandling] |  |
| `RecvblQ` |  | Latest Quarter |
| `RecvblPQ` |  | Previous Quarter |
| `RecvblPYQ` |  | Previous Quarter 1 Year Ago |
| `RecvblTTM` |  | Trailing 12 Months |
| `RecvblPTM` |  | Previous Trailing 12 Months |
| `RecvblA` |  | Latest Year |
| `RecvblPY` |  | Previous Year |
| `RecvblGr%PQ` |  | Q vs Previous Q Growth |
| `RecvblGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `RecvblGr%TTM` |  | Trailing Twelve Months Growth |
| `RecvblGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `RecvblGr%A` |  | Growth Annual |
| `RecvblGr%3Y` |  | Three Year Annualized Growth |
| `RecvblGr%5Y` |  | Five Year Annualized Growth |
| `RecvblGr%10Y` |  | Ten Year Annualized Growth |
| `RecvblRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `RecvblRSD%TTM` |  | Five Year Relative Standard Deviation |
| `RecvblRegEstANN` |  | Ten Year Regression Estimate |
| `RecvblRegEstTTM` |  | Five Year Regression Estimate |
| `RecvblRegGr%ANN` |  | Ten Year Regression Estimate |
| `RecvblRegGr%TTM` |  | Five Year Regression Growth |
| `RecvblPSQ` |  | Quarterly Per Share |
| `RecvblPSA` |  | Annual Per Share |
| `Recvbl%AssetsQ` |  | % of Quarterly Assets |
| `Recvbl%AssetsA` |  | % of Annual Assets |
| `Recvbl3YAvg` |  | Three Year Average |
| `Recvbl5YAvg` |  | Five Year Average |


#### Cash

Amount of cash and equivalents not including short-term investments.

| Factor | Params | Variant |
|--------|--------|---------|
| `Cash()` | offset, type[, NAHandling] |  |
| `CashQ` |  | Latest Quarter |
| `CashPQ` |  | Previous Quarter |
| `CashPYQ` |  | Previous Quarter 1 Year Ago |
| `CashTTM` |  | Trailing 12 Months |
| `CashPTM` |  | Previous Trailing 12 Months |
| `CashA` |  | Latest Year |
| `CashPY` |  | Previous Year |
| `CashGr%PQ` |  | Q vs Previous Q Growth |
| `CashGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashGr%TTM` |  | Trailing Twelve Months Growth |
| `CashGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashGr%A` |  | Growth Annual |
| `CashGr%3Y` |  | Three Year Annualized Growth |
| `CashGr%5Y` |  | Five Year Annualized Growth |
| `CashGr%10Y` |  | Ten Year Annualized Growth |
| `CashRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashRegEstANN` |  | Ten Year Regression Estimate |
| `CashRegEstTTM` |  | Five Year Regression Estimate |
| `CashRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashRegGr%TTM` |  | Five Year Regression Growth |
| `CashPSQ` |  | Quarterly Per Share |
| `CashPSA` |  | Annual Per Share |
| `Cash%AssetsQ` |  | % of Quarterly Assets |
| `Cash%AssetsA` |  | % of Annual Assets |
| `Cash3YAvg` |  | Three Year Average |
| `Cash5YAvg` |  | Five Year Average |


#### Cash and Equivalents

Total cash available. It includes both cash and short-term investments.

| Factor | Params | Variant |
|--------|--------|---------|
| `CashEquiv()` | offset, type[, NAHandling] |  |
| `CashEquivQ` |  | Latest Quarter |
| `CashEquivPQ` |  | Previous Quarter |
| `CashEquivPYQ` |  | Previous Quarter 1 Year Ago |
| `CashEquivTTM` |  | Trailing 12 Months |
| `CashEquivPTM` |  | Previous Trailing 12 Months |
| `CashEquivA` |  | Latest Year |
| `CashEquivPY` |  | Previous Year |
| `CashEquivGr%PQ` |  | Q vs Previous Q Growth |
| `CashEquivGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashEquivGr%TTM` |  | Trailing Twelve Months Growth |
| `CashEquivGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashEquivGr%A` |  | Growth Annual |
| `CashEquivGr%3Y` |  | Three Year Annualized Growth |
| `CashEquivGr%5Y` |  | Five Year Annualized Growth |
| `CashEquivGr%10Y` |  | Ten Year Annualized Growth |
| `CashEquivRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashEquivRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashEquivRegEstANN` |  | Ten Year Regression Estimate |
| `CashEquivRegEstTTM` |  | Five Year Regression Estimate |
| `CashEquivRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashEquivRegGr%TTM` |  | Five Year Regression Growth |
| `CashEquivPSQ` |  | Quarterly Per Share |
| `CashEquivPSA` |  | Annual Per Share |
| `CashEquiv%AssetsQ` |  | % of Quarterly Assets |
| `CashEquiv%AssetsA` |  | % of Annual Assets |
| `CashEquiv3YAvg` |  | Three Year Average |
| `CashEquiv5YAvg` |  | Five Year Average |


#### Current Assets Other

Sum of all current assets that are not included in cash, cash equivalents, short-term investments, receivables or inventory.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstCurOther()` | offset, type[, NAHandling] |  |
| `AstCurOtherQ` |  | Latest Quarter |
| `AstCurOtherPQ` |  | Previous Quarter |
| `AstCurOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `AstCurOtherTTM` |  | Trailing 12 Months |
| `AstCurOtherPTM` |  | Previous Trailing 12 Months |
| `AstCurOtherA` |  | Latest Year |
| `AstCurOtherPY` |  | Previous Year |
| `AstCurOtherGr%PQ` |  | Q vs Previous Q Growth |
| `AstCurOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstCurOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `AstCurOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstCurOtherGr%A` |  | Growth Annual |
| `AstCurOtherGr%3Y` |  | Three Year Annualized Growth |
| `AstCurOtherGr%5Y` |  | Five Year Annualized Growth |
| `AstCurOtherGr%10Y` |  | Ten Year Annualized Growth |
| `AstCurOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstCurOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstCurOtherRegEstANN` |  | Ten Year Regression Estimate |
| `AstCurOtherRegEstTTM` |  | Five Year Regression Estimate |
| `AstCurOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstCurOtherRegGr%TTM` |  | Five Year Regression Growth |
| `AstCurOtherPSQ` |  | Quarterly Per Share |
| `AstCurOtherPSA` |  | Annual Per Share |
| `AstCurOther%AssetsQ` |  | % of Quarterly Assets |
| `AstCurOther%AssetsA` |  | % of Annual Assets |
| `AstCurOther3YAvg` |  | Three Year Average |
| `AstCurOther5YAvg` |  | Five Year Average |


#### Current Assets Total

Sum of all assets expected to convert to cash within 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstCur()` | offset, type[, NAHandling] |  |
| `AstCurQ` |  | Latest Quarter |
| `AstCurPQ` |  | Previous Quarter |
| `AstCurPYQ` |  | Previous Quarter 1 Year Ago |
| `AstCurTTM` |  | Trailing 12 Months |
| `AstCurPTM` |  | Previous Trailing 12 Months |
| `AstCurA` |  | Latest Year |
| `AstCurPY` |  | Previous Year |
| `AstCurGr%PQ` |  | Q vs Previous Q Growth |
| `AstCurGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstCurGr%TTM` |  | Trailing Twelve Months Growth |
| `AstCurGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstCurGr%A` |  | Growth Annual |
| `AstCurGr%3Y` |  | Three Year Annualized Growth |
| `AstCurGr%5Y` |  | Five Year Annualized Growth |
| `AstCurGr%10Y` |  | Ten Year Annualized Growth |
| `AstCurRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstCurRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstCurRegEstANN` |  | Ten Year Regression Estimate |
| `AstCurRegEstTTM` |  | Five Year Regression Estimate |
| `AstCurRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstCurRegGr%TTM` |  | Five Year Regression Growth |
| `AstCurPSQ` |  | Quarterly Per Share |
| `AstCurPSA` |  | Annual Per Share |
| `AstCur%AssetsQ` |  | % of Quarterly Assets |
| `AstCur%AssetsA` |  | % of Annual Assets |
| `AstCur3YAvg` |  | Three Year Average |
| `AstCur5YAvg` |  | Five Year Average |


#### Inventory

Current asset representing merchandise or materials held for sale or revenue generation.

| Factor | Params | Variant |
|--------|--------|---------|
| `Inventory()` | offset, type[, NAHandling] |  |
| `InventoryQ` |  | Latest Quarter |
| `InventoryPQ` |  | Previous Quarter |
| `InventoryPYQ` |  | Previous Quarter 1 Year Ago |
| `InventoryTTM` |  | Trailing 12 Months |
| `InventoryPTM` |  | Previous Trailing 12 Months |
| `InventoryA` |  | Latest Year |
| `InventoryPY` |  | Previous Year |
| `InventoryGr%PQ` |  | Q vs Previous Q Growth |
| `InventoryGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InventoryGr%TTM` |  | Trailing Twelve Months Growth |
| `InventoryGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InventoryGr%A` |  | Growth Annual |
| `InventoryGr%3Y` |  | Three Year Annualized Growth |
| `InventoryGr%5Y` |  | Five Year Annualized Growth |
| `InventoryGr%10Y` |  | Ten Year Annualized Growth |
| `InventoryRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InventoryRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InventoryRegEstANN` |  | Ten Year Regression Estimate |
| `InventoryRegEstTTM` |  | Five Year Regression Estimate |
| `InventoryRegGr%ANN` |  | Ten Year Regression Estimate |
| `InventoryRegGr%TTM` |  | Five Year Regression Growth |
| `InventoryPSQ` |  | Quarterly Per Share |
| `InventoryPSA` |  | Annual Per Share |
| `Inventory%AssetsQ` |  | % of Quarterly Assets |
| `Inventory%AssetsA` |  | % of Annual Assets |
| `Inventory3YAvg` |  | Three Year Average |
| `Inventory5YAvg` |  | Five Year Average |


#### Short Term Investments

Current asset representing marketable securities due or expected to be traded within 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvstST()` | offset, type[, NAHandling] |  |
| `InvstSTQ` |  | Latest Quarter |
| `InvstSTPQ` |  | Previous Quarter |
| `InvstSTPYQ` |  | Previous Quarter 1 Year Ago |
| `InvstSTTTM` |  | Trailing 12 Months |
| `InvstSTPTM` |  | Previous Trailing 12 Months |
| `InvstSTA` |  | Latest Year |
| `InvstSTPY` |  | Previous Year |
| `InvstSTGr%PQ` |  | Q vs Previous Q Growth |
| `InvstSTGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvstSTGr%TTM` |  | Trailing Twelve Months Growth |
| `InvstSTGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvstSTGr%A` |  | Growth Annual |
| `InvstSTGr%3Y` |  | Three Year Annualized Growth |
| `InvstSTGr%5Y` |  | Five Year Annualized Growth |
| `InvstSTGr%10Y` |  | Ten Year Annualized Growth |
| `InvstSTRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvstSTRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvstSTRegEstANN` |  | Ten Year Regression Estimate |
| `InvstSTRegEstTTM` |  | Five Year Regression Estimate |
| `InvstSTRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvstSTRegGr%TTM` |  | Five Year Regression Growth |
| `InvstSTPSQ` |  | Quarterly Per Share |
| `InvstSTPSA` |  | Annual Per Share |
| `InvstST%AssetsQ` |  | % of Quarterly Assets |
| `InvstST%AssetsA` |  | % of Annual Assets |
| `InvstST3YAvg` |  | Three Year Average |
| `InvstST5YAvg` |  | Five Year Average |


#### Working Capital

Current assets less current liabilities.

| Factor | Params | Variant |
|--------|--------|---------|
| `WorkCap()` | offset, type[, NAHandling] |  |
| `WorkCapQ` |  | Latest Quarter |
| `WorkCapPQ` |  | Previous Quarter |
| `WorkCapPYQ` |  | Previous Quarter 1 Year Ago |
| `WorkCapTTM` |  | Trailing 12 Months |
| `WorkCapPTM` |  | Previous Trailing 12 Months |
| `WorkCapA` |  | Latest Year |
| `WorkCapPY` |  | Previous Year |
| `WorkCapGr%PQ` |  | Q vs Previous Q Growth |
| `WorkCapGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `WorkCapGr%TTM` |  | Trailing Twelve Months Growth |
| `WorkCapGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `WorkCapGr%A` |  | Growth Annual |
| `WorkCapGr%3Y` |  | Three Year Annualized Growth |
| `WorkCapGr%5Y` |  | Five Year Annualized Growth |
| `WorkCapGr%10Y` |  | Ten Year Annualized Growth |
| `WorkCapRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `WorkCapRSD%TTM` |  | Five Year Relative Standard Deviation |
| `WorkCapRegEstANN` |  | Ten Year Regression Estimate |
| `WorkCapRegEstTTM` |  | Five Year Regression Estimate |
| `WorkCapRegGr%ANN` |  | Ten Year Regression Estimate |
| `WorkCapRegGr%TTM` |  | Five Year Regression Growth |
| `WorkCapPSQ` |  | Quarterly Per Share |
| `WorkCapPSA` |  | Annual Per Share |
| `WorkCap%AssetsQ` |  | % of Quarterly Assets |
| `WorkCap%AssetsA` |  | % of Annual Assets |
| `WorkCap3YAvg` |  | Three Year Average |
| `WorkCap5YAvg` |  | Five Year Average |


### Assets-Noncurrent

Owned items that are identified by the company as being illiquid.

#### Accumulated Depreciation

Total depreciation recognized on gross property, plant and equipment (GrossPlant).

| Factor | Params | Variant |
|--------|--------|---------|
| `AccumDep()` | offset, type[, NAHandling] |  |
| `AccumDepQ` |  | Latest Quarter |
| `AccumDepPQ` |  | Previous Quarter |
| `AccumDepPYQ` |  | Previous Quarter 1 Year Ago |
| `AccumDepTTM` |  | Trailing 12 Months |
| `AccumDepPTM` |  | Previous Trailing 12 Months |
| `AccumDepA` |  | Latest Year |
| `AccumDepPY` |  | Previous Year |
| `AccumDepGr%PQ` |  | Q vs Previous Q Growth |
| `AccumDepGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AccumDepGr%TTM` |  | Trailing Twelve Months Growth |
| `AccumDepGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AccumDepGr%A` |  | Growth Annual |
| `AccumDepGr%3Y` |  | Three Year Annualized Growth |
| `AccumDepGr%5Y` |  | Five Year Annualized Growth |
| `AccumDepGr%10Y` |  | Ten Year Annualized Growth |
| `AccumDepRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AccumDepRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AccumDepRegEstANN` |  | Ten Year Regression Estimate |
| `AccumDepRegEstTTM` |  | Five Year Regression Estimate |
| `AccumDepRegGr%ANN` |  | Ten Year Regression Estimate |
| `AccumDepRegGr%TTM` |  | Five Year Regression Growth |
| `AccumDepPSQ` |  | Quarterly Per Share |
| `AccumDepPSA` |  | Annual Per Share |
| `AccumDep%AssetsQ` |  | % of Quarterly Assets |
| `AccumDep%AssetsA` |  | % of Annual Assets |
| `AccumDep3YAvg` |  | Three Year Average |
| `AccumDep5YAvg` |  | Five Year Average |


#### Equity Investments

Long-term equity investments.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvstEq()` | offset, type[, NAHandling] |  |
| `InvstEqQ` |  | Latest Quarter |
| `InvstEqPQ` |  | Previous Quarter |
| `InvstEqPYQ` |  | Previous Quarter 1 Year Ago |
| `InvstEqTTM` |  | Trailing 12 Months |
| `InvstEqPTM` |  | Previous Trailing 12 Months |
| `InvstEqA` |  | Latest Year |
| `InvstEqPY` |  | Previous Year |
| `InvstEqGr%PQ` |  | Q vs Previous Q Growth |
| `InvstEqGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvstEqGr%TTM` |  | Trailing Twelve Months Growth |
| `InvstEqGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvstEqGr%A` |  | Growth Annual |
| `InvstEqGr%3Y` |  | Three Year Annualized Growth |
| `InvstEqGr%5Y` |  | Five Year Annualized Growth |
| `InvstEqGr%10Y` |  | Ten Year Annualized Growth |
| `InvstEqRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvstEqRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvstEqRegEstANN` |  | Ten Year Regression Estimate |
| `InvstEqRegEstTTM` |  | Five Year Regression Estimate |
| `InvstEqRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvstEqRegGr%TTM` |  | Five Year Regression Growth |
| `InvstEqPSQ` |  | Quarterly Per Share |
| `InvstEqPSA` |  | Annual Per Share |
| `InvstEq%AssetsQ` |  | % of Quarterly Assets |
| `InvstEq%AssetsA` |  | % of Annual Assets |
| `InvstEq3YAvg` |  | Three Year Average |
| `InvstEq5YAvg` |  | Five Year Average |


#### Goodwill

Excess cost over equity in acquisitions.

| Factor | Params | Variant |
|--------|--------|---------|
| `Goodwill()` | offset, type[, NAHandling] |  |
| `GoodwillQ` |  | Latest Quarter |
| `GoodwillPQ` |  | Previous Quarter |
| `GoodwillPYQ` |  | Previous Quarter 1 Year Ago |
| `GoodwillTTM` |  | Trailing 12 Months |
| `GoodwillPTM` |  | Previous Trailing 12 Months |
| `GoodwillA` |  | Latest Year |
| `GoodwillPY` |  | Previous Year |
| `GoodwillGr%PQ` |  | Q vs Previous Q Growth |
| `GoodwillGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GoodwillGr%TTM` |  | Trailing Twelve Months Growth |
| `GoodwillGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GoodwillGr%A` |  | Growth Annual |
| `GoodwillGr%3Y` |  | Three Year Annualized Growth |
| `GoodwillGr%5Y` |  | Five Year Annualized Growth |
| `GoodwillGr%10Y` |  | Ten Year Annualized Growth |
| `GoodwillRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GoodwillRSD%TTM` |  | Five Year Relative Standard Deviation |
| `GoodwillRegEstANN` |  | Ten Year Regression Estimate |
| `GoodwillRegEstTTM` |  | Five Year Regression Estimate |
| `GoodwillRegGr%ANN` |  | Ten Year Regression Estimate |
| `GoodwillRegGr%TTM` |  | Five Year Regression Growth |
| `GoodwillPSQ` |  | Quarterly Per Share |
| `GoodwillPSA` |  | Annual Per Share |
| `Goodwill%AssetsQ` |  | % of Quarterly Assets |
| `Goodwill%AssetsA` |  | % of Annual Assets |
| `Goodwill3YAvg` |  | Three Year Average |
| `Goodwill5YAvg` |  | Five Year Average |


#### Gross Property Plant and Equipment

Total value of physical assets owned before depreciation adjustments.

| Factor | Params | Variant |
|--------|--------|---------|
| `GrossPlant()` | offset, type[, NAHandling] |  |
| `GrossPlantQ` |  | Latest Quarter |
| `GrossPlantPQ` |  | Previous Quarter |
| `GrossPlantPYQ` |  | Previous Quarter 1 Year Ago |
| `GrossPlantTTM` |  | Trailing 12 Months |
| `GrossPlantPTM` |  | Previous Trailing 12 Months |
| `GrossPlantA` |  | Latest Year |
| `GrossPlantPY` |  | Previous Year |
| `GrossPlantGr%PQ` |  | Q vs Previous Q Growth |
| `GrossPlantGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `GrossPlantGr%TTM` |  | Trailing Twelve Months Growth |
| `GrossPlantGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `GrossPlantGr%A` |  | Growth Annual |
| `GrossPlantGr%3Y` |  | Three Year Annualized Growth |
| `GrossPlantGr%5Y` |  | Five Year Annualized Growth |
| `GrossPlantGr%10Y` |  | Ten Year Annualized Growth |
| `GrossPlantRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `GrossPlantRSD%TTM` |  | Five Year Relative Standard Deviation |
| `GrossPlantRegEstANN` |  | Ten Year Regression Estimate |
| `GrossPlantRegEstTTM` |  | Five Year Regression Estimate |
| `GrossPlantRegGr%ANN` |  | Ten Year Regression Estimate |
| `GrossPlantRegGr%TTM` |  | Five Year Regression Growth |
| `GrossPlantPSQ` |  | Quarterly Per Share |
| `GrossPlantPSA` |  | Annual Per Share |
| `GrossPlant%AssetsQ` |  | % of Quarterly Assets |
| `GrossPlant%AssetsA` |  | % of Annual Assets |
| `GrossPlant3YAvg` |  | Three Year Average |
| `GrossPlant5YAvg` |  | Five Year Average |


#### Intangible Assets

Sum of assets that are not included in the tangible assets of property, plant and equipment.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstIntan()` | offset, type[, NAHandling] |  |
| `AstIntanQ` |  | Latest Quarter |
| `AstIntanPQ` |  | Previous Quarter |
| `AstIntanPYQ` |  | Previous Quarter 1 Year Ago |
| `AstIntanTTM` |  | Trailing 12 Months |
| `AstIntanPTM` |  | Previous Trailing 12 Months |
| `AstIntanA` |  | Latest Year |
| `AstIntanPY` |  | Previous Year |
| `AstIntanGr%PQ` |  | Q vs Previous Q Growth |
| `AstIntanGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstIntanGr%TTM` |  | Trailing Twelve Months Growth |
| `AstIntanGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstIntanGr%A` |  | Growth Annual |
| `AstIntanGr%3Y` |  | Three Year Annualized Growth |
| `AstIntanGr%5Y` |  | Five Year Annualized Growth |
| `AstIntanGr%10Y` |  | Ten Year Annualized Growth |
| `AstIntanRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstIntanRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstIntanRegEstANN` |  | Ten Year Regression Estimate |
| `AstIntanRegEstTTM` |  | Five Year Regression Estimate |
| `AstIntanRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstIntanRegGr%TTM` |  | Five Year Regression Growth |
| `AstIntanPSQ` |  | Quarterly Per Share |
| `AstIntanPSA` |  | Annual Per Share |
| `AstIntan%AssetsQ` |  | % of Quarterly Assets |
| `AstIntan%AssetsA` |  | % of Annual Assets |
| `AstIntan3YAvg` |  | Three Year Average |
| `AstIntan5YAvg` |  | Five Year Average |


#### Investments and Advances Other

Long-term receivables including investments in unconsolidated companies.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvstAdvOther()` | offset, type[, NAHandling] |  |
| `InvstAdvOtherQ` |  | Latest Quarter |
| `InvstAdvOtherPQ` |  | Previous Quarter |
| `InvstAdvOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `InvstAdvOtherTTM` |  | Trailing 12 Months |
| `InvstAdvOtherPTM` |  | Previous Trailing 12 Months |
| `InvstAdvOtherA` |  | Latest Year |
| `InvstAdvOtherPY` |  | Previous Year |
| `InvstAdvOtherGr%PQ` |  | Q vs Previous Q Growth |
| `InvstAdvOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvstAdvOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `InvstAdvOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvstAdvOtherGr%A` |  | Growth Annual |
| `InvstAdvOtherGr%3Y` |  | Three Year Annualized Growth |
| `InvstAdvOtherGr%5Y` |  | Five Year Annualized Growth |
| `InvstAdvOtherGr%10Y` |  | Ten Year Annualized Growth |
| `InvstAdvOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvstAdvOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvstAdvOtherRegEstANN` |  | Ten Year Regression Estimate |
| `InvstAdvOtherRegEstTTM` |  | Five Year Regression Estimate |
| `InvstAdvOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvstAdvOtherRegGr%TTM` |  | Five Year Regression Growth |
| `InvstAdvOtherPSQ` |  | Quarterly Per Share |
| `InvstAdvOtherPSA` |  | Annual Per Share |
| `InvstAdvOther%AssetsQ` |  | % of Quarterly Assets |
| `InvstAdvOther%AssetsA` |  | % of Annual Assets |
| `InvstAdvOther3YAvg` |  | Three Year Average |
| `InvstAdvOther5YAvg` |  | Five Year Average |


#### Net Property Plant and Equipment

Total physical assets minus accumulated depreciation.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetPlant()` | offset, type[, NAHandling] |  |
| `NetPlantQ` |  | Latest Quarter |
| `NetPlantPQ` |  | Previous Quarter |
| `NetPlantPYQ` |  | Previous Quarter 1 Year Ago |
| `NetPlantTTM` |  | Trailing 12 Months |
| `NetPlantPTM` |  | Previous Trailing 12 Months |
| `NetPlantA` |  | Latest Year |
| `NetPlantPY` |  | Previous Year |
| `NetPlantGr%PQ` |  | Q vs Previous Q Growth |
| `NetPlantGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetPlantGr%TTM` |  | Trailing Twelve Months Growth |
| `NetPlantGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetPlantGr%A` |  | Growth Annual |
| `NetPlantGr%3Y` |  | Three Year Annualized Growth |
| `NetPlantGr%5Y` |  | Five Year Annualized Growth |
| `NetPlantGr%10Y` |  | Ten Year Annualized Growth |
| `NetPlantRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetPlantRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetPlantRegEstANN` |  | Ten Year Regression Estimate |
| `NetPlantRegEstTTM` |  | Five Year Regression Estimate |
| `NetPlantRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetPlantRegGr%TTM` |  | Five Year Regression Growth |
| `NetPlantPSQ` |  | Quarterly Per Share |
| `NetPlantPSA` |  | Annual Per Share |
| `NetPlant%AssetsQ` |  | % of Quarterly Assets |
| `NetPlant%AssetsA` |  | % of Annual Assets |
| `NetPlant3YAvg` |  | Three Year Average |
| `NetPlant5YAvg` |  | Five Year Average |


#### Non-Current Assets Other

Value of assets that do not fit into either current assets or property plant and equipment.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstNonCurOther()` | offset, type[, NAHandling] |  |
| `AstNonCurOtherQ` |  | Latest Quarter |
| `AstNonCurOtherPQ` |  | Previous Quarter |
| `AstNonCurOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `AstNonCurOtherTTM` |  | Trailing 12 Months |
| `AstNonCurOtherPTM` |  | Previous Trailing 12 Months |
| `AstNonCurOtherA` |  | Latest Year |
| `AstNonCurOtherPY` |  | Previous Year |
| `AstNonCurOtherGr%PQ` |  | Q vs Previous Q Growth |
| `AstNonCurOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstNonCurOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `AstNonCurOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstNonCurOtherGr%A` |  | Growth Annual |
| `AstNonCurOtherGr%3Y` |  | Three Year Annualized Growth |
| `AstNonCurOtherGr%5Y` |  | Five Year Annualized Growth |
| `AstNonCurOtherGr%10Y` |  | Ten Year Annualized Growth |
| `AstNonCurOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstNonCurOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstNonCurOtherRegEstANN` |  | Ten Year Regression Estimate |
| `AstNonCurOtherRegEstTTM` |  | Five Year Regression Estimate |
| `AstNonCurOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstNonCurOtherRegGr%TTM` |  | Five Year Regression Growth |
| `AstNonCurOtherPSQ` |  | Quarterly Per Share |
| `AstNonCurOtherPSA` |  | Annual Per Share |
| `AstNonCurOther%AssetsQ` |  | % of Quarterly Assets |
| `AstNonCurOther%AssetsA` |  | % of Annual Assets |
| `AstNonCurOther3YAvg` |  | Three Year Average |
| `AstNonCurOther5YAvg` |  | Five Year Average |


#### Other Intangibles

All non-classifiable assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `IntanOther()` | offset, type[, NAHandling] |  |
| `IntanOtherQ` |  | Latest Quarter |
| `IntanOtherPQ` |  | Previous Quarter |
| `IntanOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `IntanOtherTTM` |  | Trailing 12 Months |
| `IntanOtherPTM` |  | Previous Trailing 12 Months |
| `IntanOtherA` |  | Latest Year |
| `IntanOtherPY` |  | Previous Year |
| `IntanOtherGr%PQ` |  | Q vs Previous Q Growth |
| `IntanOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `IntanOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `IntanOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `IntanOtherGr%A` |  | Growth Annual |
| `IntanOtherGr%3Y` |  | Three Year Annualized Growth |
| `IntanOtherGr%5Y` |  | Five Year Annualized Growth |
| `IntanOtherGr%10Y` |  | Ten Year Annualized Growth |
| `IntanOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `IntanOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `IntanOtherRegEstANN` |  | Ten Year Regression Estimate |
| `IntanOtherRegEstTTM` |  | Five Year Regression Estimate |
| `IntanOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `IntanOtherRegGr%TTM` |  | Five Year Regression Growth |
| `IntanOtherPSQ` |  | Quarterly Per Share |
| `IntanOtherPSA` |  | Annual Per Share |
| `IntanOther%AssetsQ` |  | % of Quarterly Assets |
| `IntanOther%AssetsA` |  | % of Annual Assets |
| `IntanOther3YAvg` |  | Three Year Average |
| `IntanOther5YAvg` |  | Five Year Average |


#### Total Assets

Total value of assets as reported on the balance sheet.

| Factor | Params | Variant |
|--------|--------|---------|
| `AstTot()` | offset, type[, NAHandling] |  |
| `AstTotQ` |  | Latest Quarter |
| `AstTotPQ` |  | Previous Quarter |
| `AstTotPYQ` |  | Previous Quarter 1 Year Ago |
| `AstTotTTM` |  | Trailing 12 Months |
| `AstTotPTM` |  | Previous Trailing 12 Months |
| `AstTotA` |  | Latest Year |
| `AstTotPY` |  | Previous Year |
| `AstTotGr%PQ` |  | Q vs Previous Q Growth |
| `AstTotGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AstTotGr%TTM` |  | Trailing Twelve Months Growth |
| `AstTotGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AstTotGr%A` |  | Growth Annual |
| `AstTotGr%3Y` |  | Three Year Annualized Growth |
| `AstTotGr%5Y` |  | Five Year Annualized Growth |
| `AstTotGr%10Y` |  | Ten Year Annualized Growth |
| `AstTotRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AstTotRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AstTotRegEstANN` |  | Ten Year Regression Estimate |
| `AstTotRegEstTTM` |  | Five Year Regression Estimate |
| `AstTotRegGr%ANN` |  | Ten Year Regression Estimate |
| `AstTotRegGr%TTM` |  | Five Year Regression Growth |
| `AstTotPSQ` |  | Quarterly Per Share |
| `AstTotPSA` |  | Annual Per Share |
| `AstTot%AssetsQ` |  | % of Quarterly Assets |
| `AstTot%AssetsA` |  | % of Annual Assets |
| `AstTot3YAvg` |  | Three Year Average |
| `AstTot5YAvg` |  | Five Year Average |


### Liabilities-Current

Debts that are identified by the company as due within the next 12 months.

#### Accounts Payable

Money owed by the company due within 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `Payables()` | offset, type[, NAHandling] |  |
| `PayablesQ` |  | Latest Quarter |
| `PayablesPQ` |  | Previous Quarter |
| `PayablesPYQ` |  | Previous Quarter 1 Year Ago |
| `PayablesTTM` |  | Trailing 12 Months |
| `PayablesPTM` |  | Previous Trailing 12 Months |
| `PayablesA` |  | Latest Year |
| `PayablesPY` |  | Previous Year |
| `PayablesGr%PQ` |  | Q vs Previous Q Growth |
| `PayablesGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PayablesGr%TTM` |  | Trailing Twelve Months Growth |
| `PayablesGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PayablesGr%A` |  | Growth Annual |
| `PayablesGr%3Y` |  | Three Year Annualized Growth |
| `PayablesGr%5Y` |  | Five Year Annualized Growth |
| `PayablesGr%10Y` |  | Ten Year Annualized Growth |
| `PayablesRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PayablesRSD%TTM` |  | Five Year Relative Standard Deviation |
| `PayablesRegEstANN` |  | Ten Year Regression Estimate |
| `PayablesRegEstTTM` |  | Five Year Regression Estimate |
| `PayablesRegGr%ANN` |  | Ten Year Regression Estimate |
| `PayablesRegGr%TTM` |  | Five Year Regression Growth |
| `PayablesPSQ` |  | Quarterly Per Share |
| `PayablesPSA` |  | Annual Per Share |
| `Payables%AssetsQ` |  | % of Quarterly Assets |
| `Payables%AssetsA` |  | % of Annual Assets |
| `Payables3YAvg` |  | Three Year Average |
| `Payables5YAvg` |  | Five Year Average |


#### Current Liabilities Other

All non-debt, non-payables liabilities due within 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `LiabCurOther()` | offset, type[, NAHandling] |  |
| `LiabCurOtherQ` |  | Latest Quarter |
| `LiabCurOtherPQ` |  | Previous Quarter |
| `LiabCurOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `LiabCurOtherTTM` |  | Trailing 12 Months |
| `LiabCurOtherPTM` |  | Previous Trailing 12 Months |
| `LiabCurOtherA` |  | Latest Year |
| `LiabCurOtherPY` |  | Previous Year |
| `LiabCurOtherGr%PQ` |  | Q vs Previous Q Growth |
| `LiabCurOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `LiabCurOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `LiabCurOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `LiabCurOtherGr%A` |  | Growth Annual |
| `LiabCurOtherGr%3Y` |  | Three Year Annualized Growth |
| `LiabCurOtherGr%5Y` |  | Five Year Annualized Growth |
| `LiabCurOtherGr%10Y` |  | Ten Year Annualized Growth |
| `LiabCurOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `LiabCurOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `LiabCurOtherRegEstANN` |  | Ten Year Regression Estimate |
| `LiabCurOtherRegEstTTM` |  | Five Year Regression Estimate |
| `LiabCurOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `LiabCurOtherRegGr%TTM` |  | Five Year Regression Growth |
| `LiabCurOtherPSQ` |  | Quarterly Per Share |
| `LiabCurOtherPSA` |  | Annual Per Share |
| `LiabCurOther%AssetsQ` |  | % of Quarterly Assets |
| `LiabCurOther%AssetsA` |  | % of Annual Assets |
| `LiabCurOther3YAvg` |  | Three Year Average |
| `LiabCurOther5YAvg` |  | Five Year Average |


#### Current Liabilities Total

Total liabilities due within 12 months of the balance sheet date.

| Factor | Params | Variant |
|--------|--------|---------|
| `LiabCur()` | offset, type[, NAHandling] |  |
| `LiabCurQ` |  | Latest Quarter |
| `LiabCurPQ` |  | Previous Quarter |
| `LiabCurPYQ` |  | Previous Quarter 1 Year Ago |
| `LiabCurTTM` |  | Trailing 12 Months |
| `LiabCurPTM` |  | Previous Trailing 12 Months |
| `LiabCurA` |  | Latest Year |
| `LiabCurPY` |  | Previous Year |
| `LiabCurGr%PQ` |  | Q vs Previous Q Growth |
| `LiabCurGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `LiabCurGr%TTM` |  | Trailing Twelve Months Growth |
| `LiabCurGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `LiabCurGr%A` |  | Growth Annual |
| `LiabCurGr%3Y` |  | Three Year Annualized Growth |
| `LiabCurGr%5Y` |  | Five Year Annualized Growth |
| `LiabCurGr%10Y` |  | Ten Year Annualized Growth |
| `LiabCurRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `LiabCurRSD%TTM` |  | Five Year Relative Standard Deviation |
| `LiabCurRegEstANN` |  | Ten Year Regression Estimate |
| `LiabCurRegEstTTM` |  | Five Year Regression Estimate |
| `LiabCurRegGr%ANN` |  | Ten Year Regression Estimate |
| `LiabCurRegGr%TTM` |  | Five Year Regression Growth |
| `LiabCurPSQ` |  | Quarterly Per Share |
| `LiabCurPSA` |  | Annual Per Share |
| `LiabCur%AssetsQ` |  | % of Quarterly Assets |
| `LiabCur%AssetsA` |  | % of Annual Assets |
| `LiabCur3YAvg` |  | Three Year Average |
| `LiabCur5YAvg` |  | Five Year Average |


#### Short Term Debt

Debt due within 12 months, reported as current liability on balance sheet.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtST()` | offset, type[, NAHandling] |  |
| `DbtSTQ` |  | Latest Quarter |
| `DbtSTPQ` |  | Previous Quarter |
| `DbtSTPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtSTTTM` |  | Trailing 12 Months |
| `DbtSTPTM` |  | Previous Trailing 12 Months |
| `DbtSTA` |  | Latest Year |
| `DbtSTPY` |  | Previous Year |
| `DbtSTGr%PQ` |  | Q vs Previous Q Growth |
| `DbtSTGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtSTGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtSTGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtSTGr%A` |  | Growth Annual |
| `DbtSTGr%3Y` |  | Three Year Annualized Growth |
| `DbtSTGr%5Y` |  | Five Year Annualized Growth |
| `DbtSTGr%10Y` |  | Ten Year Annualized Growth |
| `DbtSTRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtSTRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtSTRegEstANN` |  | Ten Year Regression Estimate |
| `DbtSTRegEstTTM` |  | Five Year Regression Estimate |
| `DbtSTRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtSTRegGr%TTM` |  | Five Year Regression Growth |
| `DbtSTPSQ` |  | Quarterly Per Share |
| `DbtSTPSA` |  | Annual Per Share |
| `DbtST%AssetsQ` |  | % of Quarterly Assets |
| `DbtST%AssetsA` |  | % of Annual Assets |
| `DbtST3YAvg` |  | Three Year Average |
| `DbtST5YAvg` |  | Five Year Average |


#### Taxes Payable

Current liability for taxes owed within 12 months of balance sheet date.

| Factor | Params | Variant |
|--------|--------|---------|
| `TxPayable()` | offset, type[, NAHandling] |  |
| `TxPayableQ` |  | Latest Quarter |
| `TxPayablePQ` |  | Previous Quarter |
| `TxPayablePYQ` |  | Previous Quarter 1 Year Ago |
| `TxPayableTTM` |  | Trailing 12 Months |
| `TxPayablePTM` |  | Previous Trailing 12 Months |
| `TxPayableA` |  | Latest Year |
| `TxPayablePY` |  | Previous Year |
| `TxPayableGr%PQ` |  | Q vs Previous Q Growth |
| `TxPayableGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TxPayableGr%TTM` |  | Trailing Twelve Months Growth |
| `TxPayableGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TxPayableGr%A` |  | Growth Annual |
| `TxPayableGr%3Y` |  | Three Year Annualized Growth |
| `TxPayableGr%5Y` |  | Five Year Annualized Growth |
| `TxPayableGr%10Y` |  | Ten Year Annualized Growth |
| `TxPayableRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TxPayableRSD%TTM` |  | Five Year Relative Standard Deviation |
| `TxPayableRegEstANN` |  | Ten Year Regression Estimate |
| `TxPayableRegEstTTM` |  | Five Year Regression Estimate |
| `TxPayableRegGr%ANN` |  | Ten Year Regression Estimate |
| `TxPayableRegGr%TTM` |  | Five Year Regression Growth |
| `TxPayablePSQ` |  | Quarterly Per Share |
| `TxPayablePSA` |  | Annual Per Share |
| `TxPayable%AssetsQ` |  | % of Quarterly Assets |
| `TxPayable%AssetsA` |  | % of Annual Assets |
| `TxPayable3YAvg` |  | Three Year Average |
| `TxPayable5YAvg` |  | Five Year Average |


### Liabilities-Noncurrent

Debts that are identified by the company as due more than 12 months in the future.

#### Capital Lease Obligations

Represents all obligations incurred through the contractual leasing of long-term assets, by which the periodic lease payments resemble payments on interest and debt capital. As such, capitalized leases are considered to be a form of long-term debt.

| Factor | Params | Variant |
|--------|--------|---------|
| `CapLease()` | offset, type[, NAHandling] |  |
| `CapLeaseQ` |  | Latest Quarter |
| `CapLeasePQ` |  | Previous Quarter |
| `CapLeasePYQ` |  | Previous Quarter 1 Year Ago |
| `CapLeaseTTM` |  | Trailing 12 Months |
| `CapLeasePTM` |  | Previous Trailing 12 Months |
| `CapLeaseA` |  | Latest Year |
| `CapLeasePY` |  | Previous Year |
| `CapLeaseGr%PQ` |  | Q vs Previous Q Growth |
| `CapLeaseGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CapLeaseGr%TTM` |  | Trailing Twelve Months Growth |
| `CapLeaseGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CapLeaseGr%A` |  | Growth Annual |
| `CapLeaseGr%3Y` |  | Three Year Annualized Growth |
| `CapLeaseGr%5Y` |  | Five Year Annualized Growth |
| `CapLeaseGr%10Y` |  | Ten Year Annualized Growth |
| `CapLeaseRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CapLeaseRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CapLeaseRegEstANN` |  | Ten Year Regression Estimate |
| `CapLeaseRegEstTTM` |  | Five Year Regression Estimate |
| `CapLeaseRegGr%ANN` |  | Ten Year Regression Estimate |
| `CapLeaseRegGr%TTM` |  | Five Year Regression Growth |
| `CapLeasePSQ` |  | Quarterly Per Share |
| `CapLeasePSA` |  | Annual Per Share |
| `CapLease%AssetsQ` |  | % of Quarterly Assets |
| `CapLease%AssetsA` |  | % of Annual Assets |
| `CapLease3YAvg` |  | Three Year Average |
| `CapLease5YAvg` |  | Five Year Average |


#### Deferred Taxes and Investment Credits

Accumulated deferred taxes from timing differences plus investment tax credits.

| Factor | Params | Variant |
|--------|--------|---------|
| `TxDfdIC()` | offset, type[, NAHandling] |  |
| `TxDfdICQ` |  | Latest Quarter |
| `TxDfdICPQ` |  | Previous Quarter |
| `TxDfdICPYQ` |  | Previous Quarter 1 Year Ago |
| `TxDfdICTTM` |  | Trailing 12 Months |
| `TxDfdICPTM` |  | Previous Trailing 12 Months |
| `TxDfdICA` |  | Latest Year |
| `TxDfdICPY` |  | Previous Year |
| `TxDfdICGr%PQ` |  | Q vs Previous Q Growth |
| `TxDfdICGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TxDfdICGr%TTM` |  | Trailing Twelve Months Growth |
| `TxDfdICGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TxDfdICGr%A` |  | Growth Annual |
| `TxDfdICGr%3Y` |  | Three Year Annualized Growth |
| `TxDfdICGr%5Y` |  | Five Year Annualized Growth |
| `TxDfdICGr%10Y` |  | Ten Year Annualized Growth |
| `TxDfdICRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TxDfdICRSD%TTM` |  | Five Year Relative Standard Deviation |
| `TxDfdICRegEstANN` |  | Ten Year Regression Estimate |
| `TxDfdICRegEstTTM` |  | Five Year Regression Estimate |
| `TxDfdICRegGr%ANN` |  | Ten Year Regression Estimate |
| `TxDfdICRegGr%TTM` |  | Five Year Regression Growth |
| `TxDfdICPSQ` |  | Quarterly Per Share |
| `TxDfdICPSA` |  | Annual Per Share |
| `TxDfdIC%AssetsQ` |  | % of Quarterly Assets |
| `TxDfdIC%AssetsA` |  | % of Annual Assets |
| `TxDfdIC3YAvg` |  | Three Year Average |
| `TxDfdIC5YAvg` |  | Five Year Average |


#### Long Term Debt

Debt due more than 12 months from balance sheet date.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLT()` | offset, type[, NAHandling] |  |
| `DbtLTQ` |  | Latest Quarter |
| `DbtLTPQ` |  | Previous Quarter |
| `DbtLTPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLTTTM` |  | Trailing 12 Months |
| `DbtLTPTM` |  | Previous Trailing 12 Months |
| `DbtLTA` |  | Latest Year |
| `DbtLTPY` |  | Previous Year |
| `DbtLTGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLTGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLTGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLTGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLTGr%A` |  | Growth Annual |
| `DbtLTGr%3Y` |  | Three Year Annualized Growth |
| `DbtLTGr%5Y` |  | Five Year Annualized Growth |
| `DbtLTGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLTRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLTRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLTRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLTRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLTRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLTRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLTPSQ` |  | Quarterly Per Share |
| `DbtLTPSA` |  | Annual Per Share |
| `DbtLT%AssetsQ` |  | % of Quarterly Assets |
| `DbtLT%AssetsA` |  | % of Annual Assets |
| `DbtLT3YAvg` |  | Three Year Average |
| `DbtLT5YAvg` |  | Five Year Average |


#### Other Non-current Liabilities

All long-term liabilities excluding debt, deferred taxes, investment tax credits, and minority interest.

| Factor | Params | Variant |
|--------|--------|---------|
| `LiabNonCurOther()` | offset, type[, NAHandling] |  |
| `LiabNonCurOtherQ` |  | Latest Quarter |
| `LiabNonCurOtherPQ` |  | Previous Quarter |
| `LiabNonCurOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `LiabNonCurOtherTTM` |  | Trailing 12 Months |
| `LiabNonCurOtherPTM` |  | Previous Trailing 12 Months |
| `LiabNonCurOtherA` |  | Latest Year |
| `LiabNonCurOtherPY` |  | Previous Year |
| `LiabNonCurOtherGr%PQ` |  | Q vs Previous Q Growth |
| `LiabNonCurOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `LiabNonCurOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `LiabNonCurOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `LiabNonCurOtherGr%A` |  | Growth Annual |
| `LiabNonCurOtherGr%3Y` |  | Three Year Annualized Growth |
| `LiabNonCurOtherGr%5Y` |  | Five Year Annualized Growth |
| `LiabNonCurOtherGr%10Y` |  | Ten Year Annualized Growth |
| `LiabNonCurOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `LiabNonCurOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `LiabNonCurOtherRegEstANN` |  | Ten Year Regression Estimate |
| `LiabNonCurOtherRegEstTTM` |  | Five Year Regression Estimate |
| `LiabNonCurOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `LiabNonCurOtherRegGr%TTM` |  | Five Year Regression Growth |
| `LiabNonCurOtherPSQ` |  | Quarterly Per Share |
| `LiabNonCurOtherPSA` |  | Annual Per Share |
| `LiabNonCurOther%AssetsQ` |  | % of Quarterly Assets |
| `LiabNonCurOther%AssetsA` |  | % of Annual Assets |
| `LiabNonCurOther3YAvg` |  | Three Year Average |
| `LiabNonCurOther5YAvg` |  | Five Year Average |


#### Total Debt

Sum of all debt obligations as reported on the balance sheet.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtTot()` | offset, type[, NAHandling] |  |
| `DbtTotQ` |  | Latest Quarter |
| `DbtTotPQ` |  | Previous Quarter |
| `DbtTotPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtTotTTM` |  | Trailing 12 Months |
| `DbtTotPTM` |  | Previous Trailing 12 Months |
| `DbtTotA` |  | Latest Year |
| `DbtTotPY` |  | Previous Year |
| `DbtTotGr%PQ` |  | Q vs Previous Q Growth |
| `DbtTotGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtTotGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtTotGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtTotGr%A` |  | Growth Annual |
| `DbtTotGr%3Y` |  | Three Year Annualized Growth |
| `DbtTotGr%5Y` |  | Five Year Annualized Growth |
| `DbtTotGr%10Y` |  | Ten Year Annualized Growth |
| `DbtTotRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtTotRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtTotRegEstANN` |  | Ten Year Regression Estimate |
| `DbtTotRegEstTTM` |  | Five Year Regression Estimate |
| `DbtTotRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtTotRegGr%TTM` |  | Five Year Regression Growth |
| `DbtTotPSQ` |  | Quarterly Per Share |
| `DbtTotPSA` |  | Annual Per Share |
| `DbtTot%AssetsQ` |  | % of Quarterly Assets |
| `DbtTot%AssetsA` |  | % of Annual Assets |
| `DbtTot3YAvg` |  | Three Year Average |
| `DbtTot5YAvg` |  | Five Year Average |


#### Total Liabilities

Sum of all balance sheet obligations excluding shareholders equity.

| Factor | Params | Variant |
|--------|--------|---------|
| `LiabTot()` | offset, type[, NAHandling] |  |
| `LiabTotQ` |  | Latest Quarter |
| `LiabTotPQ` |  | Previous Quarter |
| `LiabTotPYQ` |  | Previous Quarter 1 Year Ago |
| `LiabTotTTM` |  | Trailing 12 Months |
| `LiabTotPTM` |  | Previous Trailing 12 Months |
| `LiabTotA` |  | Latest Year |
| `LiabTotPY` |  | Previous Year |
| `LiabTotGr%PQ` |  | Q vs Previous Q Growth |
| `LiabTotGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `LiabTotGr%TTM` |  | Trailing Twelve Months Growth |
| `LiabTotGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `LiabTotGr%A` |  | Growth Annual |
| `LiabTotGr%3Y` |  | Three Year Annualized Growth |
| `LiabTotGr%5Y` |  | Five Year Annualized Growth |
| `LiabTotGr%10Y` |  | Ten Year Annualized Growth |
| `LiabTotRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `LiabTotRSD%TTM` |  | Five Year Relative Standard Deviation |
| `LiabTotRegEstANN` |  | Ten Year Regression Estimate |
| `LiabTotRegEstTTM` |  | Five Year Regression Estimate |
| `LiabTotRegGr%ANN` |  | Ten Year Regression Estimate |
| `LiabTotRegGr%TTM` |  | Five Year Regression Growth |
| `LiabTotPSQ` |  | Quarterly Per Share |
| `LiabTotPSA` |  | Annual Per Share |
| `LiabTot%AssetsQ` |  | % of Quarterly Assets |
| `LiabTot%AssetsA` |  | % of Annual Assets |
| `LiabTot3YAvg` |  | Three Year Average |
| `LiabTot5YAvg` |  | Five Year Average |


### Shareholders Equity

The difference between total assets and total liabilities. The lines herein indicate how much more a company is worth than the the debt that it has incurred.

#### Book Value

Value of common equity excluding preferred shares and minority interests.

| Factor | Params | Variant |
|--------|--------|---------|
| `BookVal()` | offset, type[, NAHandling] |  |
| `BookValQ` |  | Latest Quarter |
| `BookValPQ` |  | Previous Quarter |
| `BookValPYQ` |  | Previous Quarter 1 Year Ago |
| `BookValTTM` |  | Trailing 12 Months |
| `BookValPTM` |  | Previous Trailing 12 Months |
| `BookValA` |  | Latest Year |
| `BookValPY` |  | Previous Year |
| `BookValGr%PQ` |  | Q vs Previous Q Growth |
| `BookValGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `BookValGr%TTM` |  | Trailing Twelve Months Growth |
| `BookValGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `BookValGr%A` |  | Growth Annual |
| `BookValGr%3Y` |  | Three Year Annualized Growth |
| `BookValGr%5Y` |  | Five Year Annualized Growth |
| `BookValGr%10Y` |  | Ten Year Annualized Growth |
| `BookValRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `BookValRSD%TTM` |  | Five Year Relative Standard Deviation |
| `BookValRegEstANN` |  | Ten Year Regression Estimate |
| `BookValRegEstTTM` |  | Five Year Regression Estimate |
| `BookValRegGr%ANN` |  | Ten Year Regression Estimate |
| `BookValRegGr%TTM` |  | Five Year Regression Growth |
| `BookValPSQ` |  | Quarterly Per Share |
| `BookValPSA` |  | Annual Per Share |
| `BookVal%AssetsQ` |  | % of Quarterly Assets |
| `BookVal%AssetsA` |  | % of Annual Assets |
| `BookVal3YAvg` |  | Three Year Average |
| `BookVal5YAvg` |  | Five Year Average |


#### Capital Surplus

Amount shareholders paid above par value for shares.

| Factor | Params | Variant |
|--------|--------|---------|
| `CapSurplus()` | offset, type[, NAHandling] |  |
| `CapSurplusQ` |  | Latest Quarter |
| `CapSurplusPQ` |  | Previous Quarter |
| `CapSurplusPYQ` |  | Previous Quarter 1 Year Ago |
| `CapSurplusTTM` |  | Trailing 12 Months |
| `CapSurplusPTM` |  | Previous Trailing 12 Months |
| `CapSurplusA` |  | Latest Year |
| `CapSurplusPY` |  | Previous Year |
| `CapSurplusGr%PQ` |  | Q vs Previous Q Growth |
| `CapSurplusGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CapSurplusGr%TTM` |  | Trailing Twelve Months Growth |
| `CapSurplusGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CapSurplusGr%A` |  | Growth Annual |
| `CapSurplusGr%3Y` |  | Three Year Annualized Growth |
| `CapSurplusGr%5Y` |  | Five Year Annualized Growth |
| `CapSurplusGr%10Y` |  | Ten Year Annualized Growth |
| `CapSurplusRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CapSurplusRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CapSurplusRegEstANN` |  | Ten Year Regression Estimate |
| `CapSurplusRegEstTTM` |  | Five Year Regression Estimate |
| `CapSurplusRegGr%ANN` |  | Ten Year Regression Estimate |
| `CapSurplusRegGr%TTM` |  | Five Year Regression Growth |
| `CapSurplusPSQ` |  | Quarterly Per Share |
| `CapSurplusPSA` |  | Annual Per Share |
| `CapSurplus%AssetsQ` |  | % of Quarterly Assets |
| `CapSurplus%AssetsA` |  | % of Annual Assets |
| `CapSurplus3YAvg` |  | Three Year Average |
| `CapSurplus5YAvg` |  | Five Year Average |


#### Common Equity

Common shareholders' ownership interest.

| Factor | Params | Variant |
|--------|--------|---------|
| `ComEq()` | offset, type[, NAHandling] |  |
| `ComEqQ` |  | Latest Quarter |
| `ComEqPQ` |  | Previous Quarter |
| `ComEqPYQ` |  | Previous Quarter 1 Year Ago |
| `ComEqTTM` |  | Trailing 12 Months |
| `ComEqPTM` |  | Previous Trailing 12 Months |
| `ComEqA` |  | Latest Year |
| `ComEqPY` |  | Previous Year |
| `ComEqGr%PQ` |  | Q vs Previous Q Growth |
| `ComEqGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ComEqGr%TTM` |  | Trailing Twelve Months Growth |
| `ComEqGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ComEqGr%A` |  | Growth Annual |
| `ComEqGr%3Y` |  | Three Year Annualized Growth |
| `ComEqGr%5Y` |  | Five Year Annualized Growth |
| `ComEqGr%10Y` |  | Ten Year Annualized Growth |
| `ComEqRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ComEqRSD%TTM` |  | Five Year Relative Standard Deviation |
| `ComEqRegEstANN` |  | Ten Year Regression Estimate |
| `ComEqRegEstTTM` |  | Five Year Regression Estimate |
| `ComEqRegGr%ANN` |  | Ten Year Regression Estimate |
| `ComEqRegGr%TTM` |  | Five Year Regression Growth |
| `ComEqPSQ` |  | Quarterly Per Share |
| `ComEqPSA` |  | Annual Per Share |
| `ComEq%AssetsQ` |  | % of Quarterly Assets |
| `ComEq%AssetsA` |  | % of Annual Assets |
| `ComEq3YAvg` |  | Three Year Average |
| `ComEq5YAvg` |  | Five Year Average |


#### Non Controlling Interest

Formerly minority interest (pre-2009).

| Factor | Params | Variant |
|--------|--------|---------|
| `NonControlInt()` | offset, type[, NAHandling] |  |
| `NonControlIntQ` |  | Latest Quarter |
| `NonControlIntPQ` |  | Previous Quarter |
| `NonControlIntPYQ` |  | Previous Quarter 1 Year Ago |
| `NonControlIntTTM` |  | Trailing 12 Months |
| `NonControlIntPTM` |  | Previous Trailing 12 Months |
| `NonControlIntA` |  | Latest Year |
| `NonControlIntPY` |  | Previous Year |
| `NonControlIntGr%PQ` |  | Q vs Previous Q Growth |
| `NonControlIntGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NonControlIntGr%TTM` |  | Trailing Twelve Months Growth |
| `NonControlIntGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NonControlIntGr%A` |  | Growth Annual |
| `NonControlIntGr%3Y` |  | Three Year Annualized Growth |
| `NonControlIntGr%5Y` |  | Five Year Annualized Growth |
| `NonControlIntGr%10Y` |  | Ten Year Annualized Growth |
| `NonControlIntRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NonControlIntRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NonControlIntRegEstANN` |  | Ten Year Regression Estimate |
| `NonControlIntRegEstTTM` |  | Five Year Regression Estimate |
| `NonControlIntRegGr%ANN` |  | Ten Year Regression Estimate |
| `NonControlIntRegGr%TTM` |  | Five Year Regression Growth |
| `NonControlIntPSQ` |  | Quarterly Per Share |
| `NonControlIntPSA` |  | Annual Per Share |
| `NonControlInt%AssetsQ` |  | % of Quarterly Assets |
| `NonControlInt%AssetsA` |  | % of Annual Assets |
| `NonControlInt3YAvg` |  | Three Year Average |
| `NonControlInt5YAvg` |  | Five Year Average |


#### Preferred Equity

Net preferred shares multiplied by par/stated value per share.

| Factor | Params | Variant |
|--------|--------|---------|
| `PfdEquity()` | offset, type[, NAHandling] |  |
| `PfdEquityQ` |  | Latest Quarter |
| `PfdEquityPQ` |  | Previous Quarter |
| `PfdEquityPYQ` |  | Previous Quarter 1 Year Ago |
| `PfdEquityTTM` |  | Trailing 12 Months |
| `PfdEquityPTM` |  | Previous Trailing 12 Months |
| `PfdEquityA` |  | Latest Year |
| `PfdEquityPY` |  | Previous Year |
| `PfdEquityGr%PQ` |  | Q vs Previous Q Growth |
| `PfdEquityGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PfdEquityGr%TTM` |  | Trailing Twelve Months Growth |
| `PfdEquityGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PfdEquityGr%A` |  | Growth Annual |
| `PfdEquityGr%3Y` |  | Three Year Annualized Growth |
| `PfdEquityGr%5Y` |  | Five Year Annualized Growth |
| `PfdEquityGr%10Y` |  | Ten Year Annualized Growth |
| `PfdEquityRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PfdEquityRSD%TTM` |  | Five Year Relative Standard Deviation |
| `PfdEquityRegEstANN` |  | Ten Year Regression Estimate |
| `PfdEquityRegEstTTM` |  | Five Year Regression Estimate |
| `PfdEquityRegGr%ANN` |  | Ten Year Regression Estimate |
| `PfdEquityRegGr%TTM` |  | Five Year Regression Growth |
| `PfdEquityPSQ` |  | Quarterly Per Share |
| `PfdEquityPSA` |  | Annual Per Share |
| `PfdEquity%AssetsQ` |  | % of Quarterly Assets |
| `PfdEquity%AssetsA` |  | % of Annual Assets |
| `PfdEquity3YAvg` |  | Three Year Average |
| `PfdEquity5YAvg` |  | Five Year Average |


#### Retained Earnings

Net income kept rather than distributed as dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `RetainedEarn()` | offset, type[, NAHandling] |  |
| `RetainedEarnQ` |  | Latest Quarter |
| `RetainedEarnPQ` |  | Previous Quarter |
| `RetainedEarnPYQ` |  | Previous Quarter 1 Year Ago |
| `RetainedEarnTTM` |  | Trailing 12 Months |
| `RetainedEarnPTM` |  | Previous Trailing 12 Months |
| `RetainedEarnA` |  | Latest Year |
| `RetainedEarnPY` |  | Previous Year |
| `RetainedEarnGr%PQ` |  | Q vs Previous Q Growth |
| `RetainedEarnGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `RetainedEarnGr%TTM` |  | Trailing Twelve Months Growth |
| `RetainedEarnGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `RetainedEarnGr%A` |  | Growth Annual |
| `RetainedEarnGr%3Y` |  | Three Year Annualized Growth |
| `RetainedEarnGr%5Y` |  | Five Year Annualized Growth |
| `RetainedEarnGr%10Y` |  | Ten Year Annualized Growth |
| `RetainedEarnRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `RetainedEarnRSD%TTM` |  | Five Year Relative Standard Deviation |
| `RetainedEarnRegEstANN` |  | Ten Year Regression Estimate |
| `RetainedEarnRegEstTTM` |  | Five Year Regression Estimate |
| `RetainedEarnRegGr%ANN` |  | Ten Year Regression Estimate |
| `RetainedEarnRegGr%TTM` |  | Five Year Regression Growth |
| `RetainedEarnPSQ` |  | Quarterly Per Share |
| `RetainedEarnPSA` |  | Annual Per Share |
| `RetainedEarn%AssetsQ` |  | % of Quarterly Assets |
| `RetainedEarn%AssetsA` |  | % of Annual Assets |
| `RetainedEarn3YAvg` |  | Three Year Average |
| `RetainedEarn5YAvg` |  | Five Year Average |


#### Shareholder's Equity Total

Total assets minus total liabilities on the balance sheet.

| Factor | Params | Variant |
|--------|--------|---------|
| `EqTot()` | offset, type[, NAHandling] |  |
| `EqTotQ` |  | Latest Quarter |
| `EqTotPQ` |  | Previous Quarter |
| `EqTotPYQ` |  | Previous Quarter 1 Year Ago |
| `EqTotTTM` |  | Trailing 12 Months |
| `EqTotPTM` |  | Previous Trailing 12 Months |
| `EqTotA` |  | Latest Year |
| `EqTotPY` |  | Previous Year |
| `EqTotGr%PQ` |  | Q vs Previous Q Growth |
| `EqTotGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EqTotGr%TTM` |  | Trailing Twelve Months Growth |
| `EqTotGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EqTotGr%A` |  | Growth Annual |
| `EqTotGr%3Y` |  | Three Year Annualized Growth |
| `EqTotGr%5Y` |  | Five Year Annualized Growth |
| `EqTotGr%10Y` |  | Ten Year Annualized Growth |
| `EqTotRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EqTotRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EqTotRegEstANN` |  | Ten Year Regression Estimate |
| `EqTotRegEstTTM` |  | Five Year Regression Estimate |
| `EqTotRegGr%ANN` |  | Ten Year Regression Estimate |
| `EqTotRegGr%TTM` |  | Five Year Regression Growth |
| `EqTotPSQ` |  | Quarterly Per Share |
| `EqTotPSA` |  | Annual Per Share |
| `EqTot%AssetsQ` |  | % of Quarterly Assets |
| `EqTot%AssetsA` |  | % of Annual Assets |
| `EqTot3YAvg` |  | Three Year Average |
| `EqTot5YAvg` |  | Five Year Average |


#### Tangible Book Value (Net Tangible Assets)

Common equity minus intangible assets.

| Factor | Params | Variant |
|--------|--------|---------|
| `TanBV()` | offset, type[, NAHandling] |  |
| `TanBVQ` |  | Latest Quarter |
| `TanBVPQ` |  | Previous Quarter |
| `TanBVPYQ` |  | Previous Quarter 1 Year Ago |
| `TanBVTTM` |  | Trailing 12 Months |
| `TanBVPTM` |  | Previous Trailing 12 Months |
| `TanBVA` |  | Latest Year |
| `TanBVPY` |  | Previous Year |
| `TanBVGr%PQ` |  | Q vs Previous Q Growth |
| `TanBVGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TanBVGr%TTM` |  | Trailing Twelve Months Growth |
| `TanBVGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TanBVGr%A` |  | Growth Annual |
| `TanBVGr%3Y` |  | Three Year Annualized Growth |
| `TanBVGr%5Y` |  | Five Year Annualized Growth |
| `TanBVGr%10Y` |  | Ten Year Annualized Growth |
| `TanBVRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TanBVRSD%TTM` |  | Five Year Relative Standard Deviation |
| `TanBVRegEstANN` |  | Ten Year Regression Estimate |
| `TanBVRegEstTTM` |  | Five Year Regression Estimate |
| `TanBVRegGr%ANN` |  | Ten Year Regression Estimate |
| `TanBVRegGr%TTM` |  | Five Year Regression Growth |
| `TanBVPSQ` |  | Quarterly Per Share |
| `TanBVPSA` |  | Annual Per Share |
| `TanBV%AssetsQ` |  | % of Quarterly Assets |
| `TanBV%AssetsA` |  | % of Annual Assets |
| `TanBV3YAvg` |  | Three Year Average |
| `TanBV5YAvg` |  | Five Year Average |


### Shares

Basic, fully diluted and most recent share counts.

#### Common Shares Most Recent

Returns the most recent common shares outstanding from a daily source. Only includes the current primary stock. See Full Description from more info

| Factor | Params | Variant |
|--------|--------|---------|
| `SharesCur()` | barsAgo |  |


#### Common Shares

Undiluted shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `Shares()` | offset, type[, NAHandling] |  |
| `SharesQ` |  | Latest Quarter |
| `SharesPQ` |  | Previous Quarter |
| `SharesPYQ` |  | Previous Quarter 1 Year Ago |
| `SharesTTM` |  | Trailing 12 Months |
| `SharesPTM` |  | Previous Trailing 12 Months |
| `SharesA` |  | Latest Year |
| `SharesPY` |  | Previous Year |
| `SharesGr%PQ` |  | Q vs Previous Q Growth |
| `SharesGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SharesGr%TTM` |  | Trailing Twelve Months Growth |
| `SharesGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SharesGr%A` |  | Growth Annual |
| `SharesGr%3Y` |  | Three Year Annualized Growth |
| `SharesGr%5Y` |  | Five Year Annualized Growth |
| `SharesGr%10Y` |  | Ten Year Annualized Growth |
| `SharesRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SharesRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SharesRegEstANN` |  | Ten Year Regression Estimate |
| `SharesRegEstTTM` |  | Five Year Regression Estimate |
| `SharesRegGr%ANN` |  | Ten Year Regression Estimate |
| `SharesRegGr%TTM` |  | Five Year Regression Growth |
| `Shares3YAvg` |  | Three Year Average |
| `Shares5YAvg` |  | Five Year Average |


#### Common Shares Fully Diluted

Fully diluted shares outstanding.

| Factor | Params | Variant |
|--------|--------|---------|
| `SharesFD()` | offset, type[, NAHandling] |  |
| `SharesFDQ` |  | Latest Quarter |
| `SharesFDPQ` |  | Previous Quarter |
| `SharesFDPYQ` |  | Previous Quarter 1 Year Ago |
| `SharesFDTTM` |  | Trailing 12 Months |
| `SharesFDPTM` |  | Previous Trailing 12 Months |
| `SharesFDA` |  | Latest Year |
| `SharesFDPY` |  | Previous Year |
| `SharesFDGr%PQ` |  | Q vs Previous Q Growth |
| `SharesFDGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `SharesFDGr%TTM` |  | Trailing Twelve Months Growth |
| `SharesFDGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `SharesFDGr%A` |  | Growth Annual |
| `SharesFDGr%3Y` |  | Three Year Annualized Growth |
| `SharesFDGr%5Y` |  | Five Year Annualized Growth |
| `SharesFDGr%10Y` |  | Ten Year Annualized Growth |
| `SharesFDRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `SharesFDRSD%TTM` |  | Five Year Relative Standard Deviation |
| `SharesFDRegEstANN` |  | Ten Year Regression Estimate |
| `SharesFDRegEstTTM` |  | Five Year Regression Estimate |
| `SharesFDRegGr%ANN` |  | Ten Year Regression Estimate |
| `SharesFDRegGr%TTM` |  | Five Year Regression Growth |
| `SharesFD3YAvg` |  | Three Year Average |
| `SharesFD5YAvg` |  | Five Year Average |


## Cash Flow Statement

Lines from the (consolidated) statement of cash flows.

### Operating

Cash flows generated by operations, including inventory changes.

#### Change in Accrued Income Taxes

Balance sheet changes in tax liabilities.

| Factor | Params | Variant |
|--------|--------|---------|
| `TxAcrudChg()` | offset, type[, NAHandling] |  |
| `TxAcrudChgQ` |  | Latest Quarter |
| `TxAcrudChgPQ` |  | Previous Quarter |
| `TxAcrudChgPYQ` |  | Previous Quarter 1 Year Ago |
| `TxAcrudChgTTM` |  | Trailing 12 Months |
| `TxAcrudChgPTM` |  | Previous Trailing 12 Months |
| `TxAcrudChgA` |  | Latest Year |
| `TxAcrudChgPY` |  | Previous Year |
| `TxAcrudChgGr%PQ` |  | Q vs Previous Q Growth |
| `TxAcrudChgGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TxAcrudChgGr%TTM` |  | Trailing Twelve Months Growth |
| `TxAcrudChgGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TxAcrudChgGr%A` |  | Growth Annual |
| `TxAcrudChgGr%3Y` |  | Three Year Annualized Growth |
| `TxAcrudChgGr%5Y` |  | Five Year Annualized Growth |
| `TxAcrudChgGr%10Y` |  | Ten Year Annualized Growth |
| `TxAcrudChgRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TxAcrudChgRSD%TTM` |  | Five Year Relative Standard Deviation |
| `TxAcrudChgRegEstANN` |  | Ten Year Regression Estimate |
| `TxAcrudChgRegEstTTM` |  | Five Year Regression Estimate |
| `TxAcrudChgRegGr%ANN` |  | Ten Year Regression Estimate |
| `TxAcrudChgRegGr%TTM` |  | Five Year Regression Growth |
| `TxAcrudChgPSQ` |  | Quarterly Per Share |
| `TxAcrudChgPSA` |  | Annual Per Share |
| `TxAcrudChg%SalesQ` |  | % of Quarterly Sales |
| `TxAcrudChg%SalesA` |  | % of Annual Sales |
| `TxAcrudChg%AssetsQ` |  | % of Quarterly Assets |
| `TxAcrudChg%AssetsA` |  | % of Annual Assets |
| `TxAcrudChg3YAvg` |  | Three Year Average |
| `TxAcrudChg5YAvg` |  | Five Year Average |


#### Change to Accounts Receivables

Changes in receivables balance over a period.

| Factor | Params | Variant |
|--------|--------|---------|
| `RecvblChg()` | offset, type[, NAHandling] |  |
| `RecvblChgQ` |  | Latest Quarter |
| `RecvblChgPQ` |  | Previous Quarter |
| `RecvblChgPYQ` |  | Previous Quarter 1 Year Ago |
| `RecvblChgTTM` |  | Trailing 12 Months |
| `RecvblChgPTM` |  | Previous Trailing 12 Months |
| `RecvblChgA` |  | Latest Year |
| `RecvblChgPY` |  | Previous Year |
| `RecvblChgGr%PQ` |  | Q vs Previous Q Growth |
| `RecvblChgGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `RecvblChgGr%TTM` |  | Trailing Twelve Months Growth |
| `RecvblChgGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `RecvblChgGr%A` |  | Growth Annual |
| `RecvblChgGr%3Y` |  | Three Year Annualized Growth |
| `RecvblChgGr%5Y` |  | Five Year Annualized Growth |
| `RecvblChgGr%10Y` |  | Ten Year Annualized Growth |
| `RecvblChgRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `RecvblChgRSD%TTM` |  | Five Year Relative Standard Deviation |
| `RecvblChgRegEstANN` |  | Ten Year Regression Estimate |
| `RecvblChgRegEstTTM` |  | Five Year Regression Estimate |
| `RecvblChgRegGr%ANN` |  | Ten Year Regression Estimate |
| `RecvblChgRegGr%TTM` |  | Five Year Regression Growth |
| `RecvblChgPSQ` |  | Quarterly Per Share |
| `RecvblChgPSA` |  | Annual Per Share |
| `RecvblChg%SalesQ` |  | % of Quarterly Sales |
| `RecvblChg%SalesA` |  | % of Annual Sales |
| `RecvblChg%AssetsQ` |  | % of Quarterly Assets |
| `RecvblChg%AssetsA` |  | % of Annual Assets |
| `RecvblChg3YAvg` |  | Three Year Average |
| `RecvblChg5YAvg` |  | Five Year Average |


#### Change to Accrued Liabilities (Accrued Expenses)

Change in accrued liabilities on a company's balance sheet.

| Factor | Params | Variant |
|--------|--------|---------|
| `AccruedExp()` | offset, type[, NAHandling] |  |
| `AccruedExpQ` |  | Latest Quarter |
| `AccruedExpPQ` |  | Previous Quarter |
| `AccruedExpPYQ` |  | Previous Quarter 1 Year Ago |
| `AccruedExpTTM` |  | Trailing 12 Months |
| `AccruedExpPTM` |  | Previous Trailing 12 Months |
| `AccruedExpA` |  | Latest Year |
| `AccruedExpPY` |  | Previous Year |
| `AccruedExpGr%PQ` |  | Q vs Previous Q Growth |
| `AccruedExpGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AccruedExpGr%TTM` |  | Trailing Twelve Months Growth |
| `AccruedExpGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AccruedExpGr%A` |  | Growth Annual |
| `AccruedExpGr%3Y` |  | Three Year Annualized Growth |
| `AccruedExpGr%5Y` |  | Five Year Annualized Growth |
| `AccruedExpGr%10Y` |  | Ten Year Annualized Growth |
| `AccruedExpRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AccruedExpRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AccruedExpRegEstANN` |  | Ten Year Regression Estimate |
| `AccruedExpRegEstTTM` |  | Five Year Regression Estimate |
| `AccruedExpRegGr%ANN` |  | Ten Year Regression Estimate |
| `AccruedExpRegGr%TTM` |  | Five Year Regression Growth |
| `AccruedExpPSQ` |  | Quarterly Per Share |
| `AccruedExpPSA` |  | Annual Per Share |
| `AccruedExp%SalesQ` |  | % of Quarterly Sales |
| `AccruedExp%SalesA` |  | % of Annual Sales |
| `AccruedExp%AssetsQ` |  | % of Quarterly Assets |
| `AccruedExp%AssetsA` |  | % of Annual Assets |
| `AccruedExp3YAvg` |  | Three Year Average |
| `AccruedExp5YAvg` |  | Five Year Average |


#### Change to Inventory

Change in current inventory account from cash flow statement.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvtyChg()` | offset, type[, NAHandling] |  |
| `InvtyChgQ` |  | Latest Quarter |
| `InvtyChgPQ` |  | Previous Quarter |
| `InvtyChgPYQ` |  | Previous Quarter 1 Year Ago |
| `InvtyChgTTM` |  | Trailing 12 Months |
| `InvtyChgPTM` |  | Previous Trailing 12 Months |
| `InvtyChgA` |  | Latest Year |
| `InvtyChgPY` |  | Previous Year |
| `InvtyChgGr%PQ` |  | Q vs Previous Q Growth |
| `InvtyChgGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvtyChgGr%TTM` |  | Trailing Twelve Months Growth |
| `InvtyChgGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvtyChgGr%A` |  | Growth Annual |
| `InvtyChgGr%3Y` |  | Three Year Annualized Growth |
| `InvtyChgGr%5Y` |  | Five Year Annualized Growth |
| `InvtyChgGr%10Y` |  | Ten Year Annualized Growth |
| `InvtyChgRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvtyChgRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvtyChgRegEstANN` |  | Ten Year Regression Estimate |
| `InvtyChgRegEstTTM` |  | Five Year Regression Estimate |
| `InvtyChgRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvtyChgRegGr%TTM` |  | Five Year Regression Growth |
| `InvtyChgPSQ` |  | Quarterly Per Share |
| `InvtyChgPSA` |  | Annual Per Share |
| `InvtyChg%SalesQ` |  | % of Quarterly Sales |
| `InvtyChg%SalesA` |  | % of Annual Sales |
| `InvtyChg%AssetsQ` |  | % of Quarterly Assets |
| `InvtyChg%AssetsA` |  | % of Annual Assets |
| `InvtyChg3YAvg` |  | Three Year Average |
| `InvtyChg5YAvg` |  | Five Year Average |


#### Change to Other Working Capital Lines

All working capital changes not captured in specific line items (inventory, accounts payable, accounts receivable).

| Factor | Params | Variant |
|--------|--------|---------|
| `OtherWCChg()` | offset, type[, NAHandling] |  |
| `OtherWCChgQ` |  | Latest Quarter |
| `OtherWCChgPQ` |  | Previous Quarter |
| `OtherWCChgPYQ` |  | Previous Quarter 1 Year Ago |
| `OtherWCChgTTM` |  | Trailing 12 Months |
| `OtherWCChgPTM` |  | Previous Trailing 12 Months |
| `OtherWCChgA` |  | Latest Year |
| `OtherWCChgPY` |  | Previous Year |
| `OtherWCChgGr%PQ` |  | Q vs Previous Q Growth |
| `OtherWCChgGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OtherWCChgGr%TTM` |  | Trailing Twelve Months Growth |
| `OtherWCChgGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OtherWCChgGr%A` |  | Growth Annual |
| `OtherWCChgGr%3Y` |  | Three Year Annualized Growth |
| `OtherWCChgGr%5Y` |  | Five Year Annualized Growth |
| `OtherWCChgGr%10Y` |  | Ten Year Annualized Growth |
| `OtherWCChgRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OtherWCChgRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OtherWCChgRegEstANN` |  | Ten Year Regression Estimate |
| `OtherWCChgRegEstTTM` |  | Five Year Regression Estimate |
| `OtherWCChgRegGr%ANN` |  | Ten Year Regression Estimate |
| `OtherWCChgRegGr%TTM` |  | Five Year Regression Growth |
| `OtherWCChgPSQ` |  | Quarterly Per Share |
| `OtherWCChgPSA` |  | Annual Per Share |
| `OtherWCChg%SalesQ` |  | % of Quarterly Sales |
| `OtherWCChg%SalesA` |  | % of Annual Sales |
| `OtherWCChg%AssetsQ` |  | % of Quarterly Assets |
| `OtherWCChg%AssetsA` |  | % of Annual Assets |
| `OtherWCChg3YAvg` |  | Three Year Average |
| `OtherWCChg5YAvg` |  | Five Year Average |


#### Change to Payables (Accounts Payable)

Change in accounts payable balance for the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `PayablesChg()` | offset, type[, NAHandling] |  |
| `PayablesChgQ` |  | Latest Quarter |
| `PayablesChgPQ` |  | Previous Quarter |
| `PayablesChgPYQ` |  | Previous Quarter 1 Year Ago |
| `PayablesChgTTM` |  | Trailing 12 Months |
| `PayablesChgPTM` |  | Previous Trailing 12 Months |
| `PayablesChgA` |  | Latest Year |
| `PayablesChgPY` |  | Previous Year |
| `PayablesChgGr%PQ` |  | Q vs Previous Q Growth |
| `PayablesChgGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `PayablesChgGr%TTM` |  | Trailing Twelve Months Growth |
| `PayablesChgGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `PayablesChgGr%A` |  | Growth Annual |
| `PayablesChgGr%3Y` |  | Three Year Annualized Growth |
| `PayablesChgGr%5Y` |  | Five Year Annualized Growth |
| `PayablesChgGr%10Y` |  | Ten Year Annualized Growth |
| `PayablesChgRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `PayablesChgRSD%TTM` |  | Five Year Relative Standard Deviation |
| `PayablesChgRegEstANN` |  | Ten Year Regression Estimate |
| `PayablesChgRegEstTTM` |  | Five Year Regression Estimate |
| `PayablesChgRegGr%ANN` |  | Ten Year Regression Estimate |
| `PayablesChgRegGr%TTM` |  | Five Year Regression Growth |
| `PayablesChgPSQ` |  | Quarterly Per Share |
| `PayablesChgPSA` |  | Annual Per Share |
| `PayablesChg%SalesQ` |  | % of Quarterly Sales |
| `PayablesChg%SalesA` |  | % of Annual Sales |
| `PayablesChg%AssetsQ` |  | % of Quarterly Assets |
| `PayablesChg%AssetsA` |  | % of Annual Assets |
| `PayablesChg3YAvg` |  | Three Year Average |
| `PayablesChg5YAvg` |  | Five Year Average |


#### Deferred Taxes

Expense from repaying deferred tax liabilities (on cash flow statement).

| Factor | Params | Variant |
|--------|--------|---------|
| `TxDfd()` | offset, type[, NAHandling] |  |
| `TxDfdQ` |  | Latest Quarter |
| `TxDfdPQ` |  | Previous Quarter |
| `TxDfdPYQ` |  | Previous Quarter 1 Year Ago |
| `TxDfdTTM` |  | Trailing 12 Months |
| `TxDfdPTM` |  | Previous Trailing 12 Months |
| `TxDfdA` |  | Latest Year |
| `TxDfdPY` |  | Previous Year |
| `TxDfdGr%PQ` |  | Q vs Previous Q Growth |
| `TxDfdGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `TxDfdGr%TTM` |  | Trailing Twelve Months Growth |
| `TxDfdGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `TxDfdGr%A` |  | Growth Annual |
| `TxDfdGr%3Y` |  | Three Year Annualized Growth |
| `TxDfdGr%5Y` |  | Five Year Annualized Growth |
| `TxDfdGr%10Y` |  | Ten Year Annualized Growth |
| `TxDfdRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `TxDfdRSD%TTM` |  | Five Year Relative Standard Deviation |
| `TxDfdRegEstANN` |  | Ten Year Regression Estimate |
| `TxDfdRegEstTTM` |  | Five Year Regression Estimate |
| `TxDfdRegGr%ANN` |  | Ten Year Regression Estimate |
| `TxDfdRegGr%TTM` |  | Five Year Regression Growth |
| `TxDfdPSQ` |  | Quarterly Per Share |
| `TxDfdPSA` |  | Annual Per Share |
| `TxDfd%SalesQ` |  | % of Quarterly Sales |
| `TxDfd%SalesA` |  | % of Annual Sales |
| `TxDfd%AssetsQ` |  | % of Quarterly Assets |
| `TxDfd%AssetsA` |  | % of Annual Assets |
| `TxDfd3YAvg` |  | Three Year Average |
| `TxDfd5YAvg` |  | Five Year Average |


#### Depreciation and Amort, Cash Flow

Depreciation and Amortization as reported on cash flow statement.

| Factor | Params | Variant |
|--------|--------|---------|
| `DepAmortCF()` | offset, type[, NAHandling] |  |
| `DepAmortCFQ` |  | Latest Quarter |
| `DepAmortCFPQ` |  | Previous Quarter |
| `DepAmortCFPYQ` |  | Previous Quarter 1 Year Ago |
| `DepAmortCFTTM` |  | Trailing 12 Months |
| `DepAmortCFPTM` |  | Previous Trailing 12 Months |
| `DepAmortCFA` |  | Latest Year |
| `DepAmortCFPY` |  | Previous Year |
| `DepAmortCFGr%PQ` |  | Q vs Previous Q Growth |
| `DepAmortCFGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DepAmortCFGr%TTM` |  | Trailing Twelve Months Growth |
| `DepAmortCFGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DepAmortCFGr%A` |  | Growth Annual |
| `DepAmortCFGr%3Y` |  | Three Year Annualized Growth |
| `DepAmortCFGr%5Y` |  | Five Year Annualized Growth |
| `DepAmortCFGr%10Y` |  | Ten Year Annualized Growth |
| `DepAmortCFRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DepAmortCFRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DepAmortCFRegEstANN` |  | Ten Year Regression Estimate |
| `DepAmortCFRegEstTTM` |  | Five Year Regression Estimate |
| `DepAmortCFRegGr%ANN` |  | Ten Year Regression Estimate |
| `DepAmortCFRegGr%TTM` |  | Five Year Regression Growth |
| `DepAmortCFPSQ` |  | Quarterly Per Share |
| `DepAmortCFPSA` |  | Annual Per Share |
| `DepAmortCF%SalesQ` |  | % of Quarterly Sales |
| `DepAmortCF%SalesA` |  | % of Annual Sales |
| `DepAmortCF%AssetsQ` |  | % of Quarterly Assets |
| `DepAmortCF%AssetsA` |  | % of Annual Assets |
| `DepAmortCF3YAvg` |  | Three Year Average |
| `DepAmortCF5YAvg` |  | Five Year Average |


#### Net Income (Cash Flow Statement)

Top line of the cash flow statement using indirect method.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetIncCFStmt()` | offset, type[, NAHandling] |  |
| `NetIncCFStmtQ` |  | Latest Quarter |
| `NetIncCFStmtPQ` |  | Previous Quarter |
| `NetIncCFStmtPYQ` |  | Previous Quarter 1 Year Ago |
| `NetIncCFStmtTTM` |  | Trailing 12 Months |
| `NetIncCFStmtPTM` |  | Previous Trailing 12 Months |
| `NetIncCFStmtA` |  | Latest Year |
| `NetIncCFStmtPY` |  | Previous Year |
| `NetIncCFStmtGr%PQ` |  | Q vs Previous Q Growth |
| `NetIncCFStmtGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetIncCFStmtGr%TTM` |  | Trailing Twelve Months Growth |
| `NetIncCFStmtGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetIncCFStmtGr%A` |  | Growth Annual |
| `NetIncCFStmtGr%3Y` |  | Three Year Annualized Growth |
| `NetIncCFStmtGr%5Y` |  | Five Year Annualized Growth |
| `NetIncCFStmtGr%10Y` |  | Ten Year Annualized Growth |
| `NetIncCFStmtRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetIncCFStmtRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetIncCFStmtRegEstANN` |  | Ten Year Regression Estimate |
| `NetIncCFStmtRegEstTTM` |  | Five Year Regression Estimate |
| `NetIncCFStmtRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetIncCFStmtRegGr%TTM` |  | Five Year Regression Growth |
| `NetIncCFStmtPSQ` |  | Quarterly Per Share |
| `NetIncCFStmtPSA` |  | Annual Per Share |
| `NetIncCFStmt%SalesQ` |  | % of Quarterly Sales |
| `NetIncCFStmt%SalesA` |  | % of Annual Sales |
| `NetIncCFStmt%AssetsQ` |  | % of Quarterly Assets |
| `NetIncCFStmt%AssetsA` |  | % of Annual Assets |
| `NetIncCFStmt3YAvg` |  | Three Year Average |
| `NetIncCFStmt5YAvg` |  | Five Year Average |


#### Operating Cash Flow from Operations

Total cash change from operating activities.

| Factor | Params | Variant |
|--------|--------|---------|
| `OperCashFl()` | offset, type[, NAHandling] |  |
| `OperCashFlQ` |  | Latest Quarter |
| `OperCashFlPQ` |  | Previous Quarter |
| `OperCashFlPYQ` |  | Previous Quarter 1 Year Ago |
| `OperCashFlTTM` |  | Trailing 12 Months |
| `OperCashFlPTM` |  | Previous Trailing 12 Months |
| `OperCashFlA` |  | Latest Year |
| `OperCashFlPY` |  | Previous Year |
| `OperCashFlGr%PQ` |  | Q vs Previous Q Growth |
| `OperCashFlGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `OperCashFlGr%TTM` |  | Trailing Twelve Months Growth |
| `OperCashFlGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `OperCashFlGr%A` |  | Growth Annual |
| `OperCashFlGr%3Y` |  | Three Year Annualized Growth |
| `OperCashFlGr%5Y` |  | Five Year Annualized Growth |
| `OperCashFlGr%10Y` |  | Ten Year Annualized Growth |
| `OperCashFlRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `OperCashFlRSD%TTM` |  | Five Year Relative Standard Deviation |
| `OperCashFlRegEstANN` |  | Ten Year Regression Estimate |
| `OperCashFlRegEstTTM` |  | Five Year Regression Estimate |
| `OperCashFlRegGr%ANN` |  | Ten Year Regression Estimate |
| `OperCashFlRegGr%TTM` |  | Five Year Regression Growth |
| `OperCashFlPSQ` |  | Quarterly Per Share |
| `OperCashFlPSA` |  | Annual Per Share |
| `OperCashFl%SalesQ` |  | % of Quarterly Sales |
| `OperCashFl%SalesA` |  | % of Annual Sales |
| `OperCashFl%AssetsQ` |  | % of Quarterly Assets |
| `OperCashFl%AssetsA` |  | % of Annual Assets |
| `OperCashFl3YAvg` |  | Three Year Average |
| `OperCashFl5YAvg` |  | Five Year Average |


#### Stock Option Compensation, Cash Flow

Cashflow statement SBC. Data begins around 2006, with full annual coverage starting in 2013, and interim in 2021

| Factor | Params | Variant |
|--------|--------|---------|
| `StkOptCF()` | offset, type[, NAHandling] |  |
| `StkOptCFQ` |  | Latest Quarter |
| `StkOptCFPQ` |  | Previous Quarter |
| `StkOptCFPYQ` |  | Previous Quarter 1 Year Ago |
| `StkOptCFTTM` |  | Trailing 12 Months |
| `StkOptCFPTM` |  | Previous Trailing 12 Months |
| `StkOptCFA` |  | Latest Year |
| `StkOptCFPY` |  | Previous Year |
| `StkOptCFGr%PQ` |  | Q vs Previous Q Growth |
| `StkOptCFGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `StkOptCFGr%TTM` |  | Trailing Twelve Months Growth |
| `StkOptCFGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `StkOptCFGr%A` |  | Growth Annual |
| `StkOptCFGr%3Y` |  | Three Year Annualized Growth |
| `StkOptCFGr%5Y` |  | Five Year Annualized Growth |
| `StkOptCFGr%10Y` |  | Ten Year Annualized Growth |
| `StkOptCFRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `StkOptCFRSD%TTM` |  | Five Year Relative Standard Deviation |
| `StkOptCFRegEstANN` |  | Ten Year Regression Estimate |
| `StkOptCFRegEstTTM` |  | Five Year Regression Estimate |
| `StkOptCFRegGr%ANN` |  | Ten Year Regression Estimate |
| `StkOptCFRegGr%TTM` |  | Five Year Regression Growth |
| `StkOptCFPSQ` |  | Quarterly Per Share |
| `StkOptCFPSA` |  | Annual Per Share |
| `StkOptCF%SalesQ` |  | % of Quarterly Sales |
| `StkOptCF%SalesA` |  | % of Annual Sales |
| `StkOptCF%AssetsQ` |  | % of Quarterly Assets |
| `StkOptCF%AssetsA` |  | % of Annual Assets |
| `StkOptCF3YAvg` |  | Three Year Average |
| `StkOptCF5YAvg` |  | Five Year Average |


### Investing

Cash flows generated by investing activities, including capital expenditures.

#### Acquisitions

Cash outflows for purchasing companies or equity stakes.

| Factor | Params | Variant |
|--------|--------|---------|
| `Acquis()` | offset, type[, NAHandling] |  |
| `AcquisQ` |  | Latest Quarter |
| `AcquisPQ` |  | Previous Quarter |
| `AcquisPYQ` |  | Previous Quarter 1 Year Ago |
| `AcquisTTM` |  | Trailing 12 Months |
| `AcquisPTM` |  | Previous Trailing 12 Months |
| `AcquisA` |  | Latest Year |
| `AcquisPY` |  | Previous Year |
| `AcquisGr%PQ` |  | Q vs Previous Q Growth |
| `AcquisGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `AcquisGr%TTM` |  | Trailing Twelve Months Growth |
| `AcquisGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `AcquisGr%A` |  | Growth Annual |
| `AcquisGr%3Y` |  | Three Year Annualized Growth |
| `AcquisGr%5Y` |  | Five Year Annualized Growth |
| `AcquisGr%10Y` |  | Ten Year Annualized Growth |
| `AcquisRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `AcquisRSD%TTM` |  | Five Year Relative Standard Deviation |
| `AcquisRegEstANN` |  | Ten Year Regression Estimate |
| `AcquisRegEstTTM` |  | Five Year Regression Estimate |
| `AcquisRegGr%ANN` |  | Ten Year Regression Estimate |
| `AcquisRegGr%TTM` |  | Five Year Regression Growth |
| `AcquisPSQ` |  | Quarterly Per Share |
| `AcquisPSA` |  | Annual Per Share |
| `Acquis%SalesQ` |  | % of Quarterly Sales |
| `Acquis%SalesA` |  | % of Annual Sales |
| `Acquis%AssetsQ` |  | % of Quarterly Assets |
| `Acquis%AssetsA` |  | % of Annual Assets |
| `Acquis3YAvg` |  | Three Year Average |
| `Acquis5YAvg` |  | Five Year Average |


#### Capital Expenditures (CapEx)

Expenditures on property, plant, and equipment investments.

| Factor | Params | Variant |
|--------|--------|---------|
| `CapEx()` | offset, type[, NAHandling] |  |
| `CapExQ` |  | Latest Quarter |
| `CapExPQ` |  | Previous Quarter |
| `CapExPYQ` |  | Previous Quarter 1 Year Ago |
| `CapExTTM` |  | Trailing 12 Months |
| `CapExPTM` |  | Previous Trailing 12 Months |
| `CapExA` |  | Latest Year |
| `CapExPY` |  | Previous Year |
| `CapExGr%PQ` |  | Q vs Previous Q Growth |
| `CapExGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CapExGr%TTM` |  | Trailing Twelve Months Growth |
| `CapExGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CapExGr%A` |  | Growth Annual |
| `CapExGr%3Y` |  | Three Year Annualized Growth |
| `CapExGr%5Y` |  | Five Year Annualized Growth |
| `CapExGr%10Y` |  | Ten Year Annualized Growth |
| `CapExRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CapExRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CapExRegEstANN` |  | Ten Year Regression Estimate |
| `CapExRegEstTTM` |  | Five Year Regression Estimate |
| `CapExRegGr%ANN` |  | Ten Year Regression Estimate |
| `CapExRegGr%TTM` |  | Five Year Regression Growth |
| `CapExPSQ` |  | Quarterly Per Share |
| `CapExPSA` |  | Annual Per Share |
| `CapEx%SalesQ` |  | % of Quarterly Sales |
| `CapEx%SalesA` |  | % of Annual Sales |
| `CapEx%AssetsQ` |  | % of Quarterly Assets |
| `CapEx%AssetsA` |  | % of Annual Assets |
| `CapEx3YAvg` |  | Three Year Average |
| `CapEx5YAvg` |  | Five Year Average |


#### Cash from Investing

Net cash flows from investing activities.

| Factor | Params | Variant |
|--------|--------|---------|
| `CashFrInvest()` | offset, type[, NAHandling] |  |
| `CashFrInvestQ` |  | Latest Quarter |
| `CashFrInvestPQ` |  | Previous Quarter |
| `CashFrInvestPYQ` |  | Previous Quarter 1 Year Ago |
| `CashFrInvestTTM` |  | Trailing 12 Months |
| `CashFrInvestPTM` |  | Previous Trailing 12 Months |
| `CashFrInvestA` |  | Latest Year |
| `CashFrInvestPY` |  | Previous Year |
| `CashFrInvestGr%PQ` |  | Q vs Previous Q Growth |
| `CashFrInvestGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashFrInvestGr%TTM` |  | Trailing Twelve Months Growth |
| `CashFrInvestGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashFrInvestGr%A` |  | Growth Annual |
| `CashFrInvestGr%3Y` |  | Three Year Annualized Growth |
| `CashFrInvestGr%5Y` |  | Five Year Annualized Growth |
| `CashFrInvestGr%10Y` |  | Ten Year Annualized Growth |
| `CashFrInvestRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashFrInvestRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashFrInvestRegEstANN` |  | Ten Year Regression Estimate |
| `CashFrInvestRegEstTTM` |  | Five Year Regression Estimate |
| `CashFrInvestRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashFrInvestRegGr%TTM` |  | Five Year Regression Growth |
| `CashFrInvestPSQ` |  | Quarterly Per Share |
| `CashFrInvestPSA` |  | Annual Per Share |
| `CashFrInvest%SalesQ` |  | % of Quarterly Sales |
| `CashFrInvest%SalesA` |  | % of Annual Sales |
| `CashFrInvest%AssetsQ` |  | % of Quarterly Assets |
| `CashFrInvest%AssetsA` |  | % of Annual Assets |
| `CashFrInvest3YAvg` |  | Three Year Average |
| `CashFrInvest5YAvg` |  | Five Year Average |


#### Divestitures

Cash inflow from selling companies/subsidiaries.

| Factor | Params | Variant |
|--------|--------|---------|
| `Divest()` | offset, type[, NAHandling] |  |
| `DivestQ` |  | Latest Quarter |
| `DivestPQ` |  | Previous Quarter |
| `DivestPYQ` |  | Previous Quarter 1 Year Ago |
| `DivestTTM` |  | Trailing 12 Months |
| `DivestPTM` |  | Previous Trailing 12 Months |
| `DivestA` |  | Latest Year |
| `DivestPY` |  | Previous Year |
| `DivestGr%PQ` |  | Q vs Previous Q Growth |
| `DivestGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DivestGr%TTM` |  | Trailing Twelve Months Growth |
| `DivestGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DivestGr%A` |  | Growth Annual |
| `DivestGr%3Y` |  | Three Year Annualized Growth |
| `DivestGr%5Y` |  | Five Year Annualized Growth |
| `DivestGr%10Y` |  | Ten Year Annualized Growth |
| `DivestRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DivestRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DivestRegEstANN` |  | Ten Year Regression Estimate |
| `DivestRegEstTTM` |  | Five Year Regression Estimate |
| `DivestRegGr%ANN` |  | Ten Year Regression Estimate |
| `DivestRegGr%TTM` |  | Five Year Regression Growth |
| `DivestPSQ` |  | Quarterly Per Share |
| `DivestPSA` |  | Annual Per Share |
| `Divest%SalesQ` |  | % of Quarterly Sales |
| `Divest%SalesA` |  | % of Annual Sales |
| `Divest%AssetsQ` |  | % of Quarterly Assets |
| `Divest%AssetsA` |  | % of Annual Assets |
| `Divest3YAvg` |  | Three Year Average |
| `Divest5YAvg` |  | Five Year Average |


#### Other Investing Cash Flow

Miscellaneous investing cash flows not classified elsewhere.

| Factor | Params | Variant |
|--------|--------|---------|
| `InvstOther()` | offset, type[, NAHandling] |  |
| `InvstOtherQ` |  | Latest Quarter |
| `InvstOtherPQ` |  | Previous Quarter |
| `InvstOtherPYQ` |  | Previous Quarter 1 Year Ago |
| `InvstOtherTTM` |  | Trailing 12 Months |
| `InvstOtherPTM` |  | Previous Trailing 12 Months |
| `InvstOtherA` |  | Latest Year |
| `InvstOtherPY` |  | Previous Year |
| `InvstOtherGr%PQ` |  | Q vs Previous Q Growth |
| `InvstOtherGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `InvstOtherGr%TTM` |  | Trailing Twelve Months Growth |
| `InvstOtherGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `InvstOtherGr%A` |  | Growth Annual |
| `InvstOtherGr%3Y` |  | Three Year Annualized Growth |
| `InvstOtherGr%5Y` |  | Five Year Annualized Growth |
| `InvstOtherGr%10Y` |  | Ten Year Annualized Growth |
| `InvstOtherRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `InvstOtherRSD%TTM` |  | Five Year Relative Standard Deviation |
| `InvstOtherRegEstANN` |  | Ten Year Regression Estimate |
| `InvstOtherRegEstTTM` |  | Five Year Regression Estimate |
| `InvstOtherRegGr%ANN` |  | Ten Year Regression Estimate |
| `InvstOtherRegGr%TTM` |  | Five Year Regression Growth |
| `InvstOtherPSQ` |  | Quarterly Per Share |
| `InvstOtherPSA` |  | Annual Per Share |
| `InvstOther%SalesQ` |  | % of Quarterly Sales |
| `InvstOther%SalesA` |  | % of Annual Sales |
| `InvstOther%AssetsQ` |  | % of Quarterly Assets |
| `InvstOther%AssetsA` |  | % of Annual Assets |
| `InvstOther3YAvg` |  | Three Year Average |
| `InvstOther5YAvg` |  | Five Year Average |


### Financing

Cash flows generated by financing activities, including debt service and dividend payments.

#### Cash From Financing

Sum of all financing activity cash flows.

| Factor | Params | Variant |
|--------|--------|---------|
| `CashFrFin()` | offset, type[, NAHandling] |  |
| `CashFrFinQ` |  | Latest Quarter |
| `CashFrFinPQ` |  | Previous Quarter |
| `CashFrFinPYQ` |  | Previous Quarter 1 Year Ago |
| `CashFrFinTTM` |  | Trailing 12 Months |
| `CashFrFinPTM` |  | Previous Trailing 12 Months |
| `CashFrFinA` |  | Latest Year |
| `CashFrFinPY` |  | Previous Year |
| `CashFrFinGr%PQ` |  | Q vs Previous Q Growth |
| `CashFrFinGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashFrFinGr%TTM` |  | Trailing Twelve Months Growth |
| `CashFrFinGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashFrFinGr%A` |  | Growth Annual |
| `CashFrFinGr%3Y` |  | Three Year Annualized Growth |
| `CashFrFinGr%5Y` |  | Five Year Annualized Growth |
| `CashFrFinGr%10Y` |  | Ten Year Annualized Growth |
| `CashFrFinRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashFrFinRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashFrFinRegEstANN` |  | Ten Year Regression Estimate |
| `CashFrFinRegEstTTM` |  | Five Year Regression Estimate |
| `CashFrFinRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashFrFinRegGr%TTM` |  | Five Year Regression Growth |
| `CashFrFinPSQ` |  | Quarterly Per Share |
| `CashFrFinPSA` |  | Annual Per Share |
| `CashFrFin%SalesQ` |  | % of Quarterly Sales |
| `CashFrFin%SalesA` |  | % of Annual Sales |
| `CashFrFin%AssetsQ` |  | % of Quarterly Assets |
| `CashFrFin%AssetsA` |  | % of Annual Assets |
| `CashFrFin3YAvg` |  | Three Year Average |
| `CashFrFin5YAvg` |  | Five Year Average |


#### Change to Debt

Net debt activity during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `ChangeDebt()` | offset, type[, NAHandling] |  |
| `ChangeDebtQ` |  | Latest Quarter |
| `ChangeDebtPQ` |  | Previous Quarter |
| `ChangeDebtPYQ` |  | Previous Quarter 1 Year Ago |
| `ChangeDebtTTM` |  | Trailing 12 Months |
| `ChangeDebtPTM` |  | Previous Trailing 12 Months |
| `ChangeDebtA` |  | Latest Year |
| `ChangeDebtPY` |  | Previous Year |
| `ChangeDebtGr%PQ` |  | Q vs Previous Q Growth |
| `ChangeDebtGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ChangeDebtGr%TTM` |  | Trailing Twelve Months Growth |
| `ChangeDebtGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ChangeDebtGr%A` |  | Growth Annual |
| `ChangeDebtGr%3Y` |  | Three Year Annualized Growth |
| `ChangeDebtGr%5Y` |  | Five Year Annualized Growth |
| `ChangeDebtGr%10Y` |  | Ten Year Annualized Growth |
| `ChangeDebtRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ChangeDebtRSD%TTM` |  | Five Year Relative Standard Deviation |
| `ChangeDebtRegEstANN` |  | Ten Year Regression Estimate |
| `ChangeDebtRegEstTTM` |  | Five Year Regression Estimate |
| `ChangeDebtRegGr%ANN` |  | Ten Year Regression Estimate |
| `ChangeDebtRegGr%TTM` |  | Five Year Regression Growth |
| `ChangeDebtPSQ` |  | Quarterly Per Share |
| `ChangeDebtPSA` |  | Annual Per Share |
| `ChangeDebt%SalesQ` |  | % of Quarterly Sales |
| `ChangeDebt%SalesA` |  | % of Annual Sales |
| `ChangeDebt%AssetsQ` |  | % of Quarterly Assets |
| `ChangeDebt%AssetsA` |  | % of Annual Assets |
| `ChangeDebt3YAvg` |  | Three Year Average |
| `ChangeDebt5YAvg` |  | Five Year Average |


#### Change to Equity

Net equity activity during the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `ChangeEq()` | offset, type[, NAHandling] |  |
| `ChangeEqQ` |  | Latest Quarter |
| `ChangeEqPQ` |  | Previous Quarter |
| `ChangeEqPYQ` |  | Previous Quarter 1 Year Ago |
| `ChangeEqTTM` |  | Trailing 12 Months |
| `ChangeEqPTM` |  | Previous Trailing 12 Months |
| `ChangeEqA` |  | Latest Year |
| `ChangeEqPY` |  | Previous Year |
| `ChangeEqGr%PQ` |  | Q vs Previous Q Growth |
| `ChangeEqGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `ChangeEqGr%TTM` |  | Trailing Twelve Months Growth |
| `ChangeEqGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `ChangeEqGr%A` |  | Growth Annual |
| `ChangeEqGr%3Y` |  | Three Year Annualized Growth |
| `ChangeEqGr%5Y` |  | Five Year Annualized Growth |
| `ChangeEqGr%10Y` |  | Ten Year Annualized Growth |
| `ChangeEqRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `ChangeEqRSD%TTM` |  | Five Year Relative Standard Deviation |
| `ChangeEqRegEstANN` |  | Ten Year Regression Estimate |
| `ChangeEqRegEstTTM` |  | Five Year Regression Estimate |
| `ChangeEqRegGr%ANN` |  | Ten Year Regression Estimate |
| `ChangeEqRegGr%TTM` |  | Five Year Regression Growth |
| `ChangeEqPSQ` |  | Quarterly Per Share |
| `ChangeEqPSA` |  | Annual Per Share |
| `ChangeEq%SalesQ` |  | % of Quarterly Sales |
| `ChangeEq%SalesA` |  | % of Annual Sales |
| `ChangeEq%AssetsQ` |  | % of Quarterly Assets |
| `ChangeEq%AssetsA` |  | % of Annual Assets |
| `ChangeEq3YAvg` |  | Three Year Average |
| `ChangeEq5YAvg` |  | Five Year Average |


#### Dividends Paid (Total Cash Flow)

Total dividends paid across all share classes and preferred shares.

| Factor | Params | Variant |
|--------|--------|---------|
| `DivPaid()` | offset, type[, NAHandling] |  |
| `DivPaidQ` |  | Latest Quarter |
| `DivPaidPQ` |  | Previous Quarter |
| `DivPaidPYQ` |  | Previous Quarter 1 Year Ago |
| `DivPaidTTM` |  | Trailing 12 Months |
| `DivPaidPTM` |  | Previous Trailing 12 Months |
| `DivPaidA` |  | Latest Year |
| `DivPaidPY` |  | Previous Year |
| `DivPaidGr%PQ` |  | Q vs Previous Q Growth |
| `DivPaidGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DivPaidGr%TTM` |  | Trailing Twelve Months Growth |
| `DivPaidGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DivPaidGr%A` |  | Growth Annual |
| `DivPaidGr%3Y` |  | Three Year Annualized Growth |
| `DivPaidGr%5Y` |  | Five Year Annualized Growth |
| `DivPaidGr%10Y` |  | Ten Year Annualized Growth |
| `DivPaidRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DivPaidRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DivPaidRegEstANN` |  | Ten Year Regression Estimate |
| `DivPaidRegEstTTM` |  | Five Year Regression Estimate |
| `DivPaidRegGr%ANN` |  | Ten Year Regression Estimate |
| `DivPaidRegGr%TTM` |  | Five Year Regression Growth |
| `DivPaidPSQ` |  | Quarterly Per Share |
| `DivPaidPSA` |  | Annual Per Share |
| `DivPaid%SalesQ` |  | % of Quarterly Sales |
| `DivPaid%SalesA` |  | % of Annual Sales |
| `DivPaid%AssetsQ` |  | % of Quarterly Assets |
| `DivPaid%AssetsA` |  | % of Annual Assets |
| `DivPaid3YAvg` |  | Three Year Average |
| `DivPaid5YAvg` |  | Five Year Average |


#### Equity Issued

Cash received from issuing equity instruments.

| Factor | Params | Variant |
|--------|--------|---------|
| `EqIssued()` | offset, type[, NAHandling] |  |
| `EqIssuedQ` |  | Latest Quarter |
| `EqIssuedPQ` |  | Previous Quarter |
| `EqIssuedPYQ` |  | Previous Quarter 1 Year Ago |
| `EqIssuedTTM` |  | Trailing 12 Months |
| `EqIssuedPTM` |  | Previous Trailing 12 Months |
| `EqIssuedA` |  | Latest Year |
| `EqIssuedPY` |  | Previous Year |
| `EqIssuedGr%PQ` |  | Q vs Previous Q Growth |
| `EqIssuedGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EqIssuedGr%TTM` |  | Trailing Twelve Months Growth |
| `EqIssuedGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EqIssuedGr%A` |  | Growth Annual |
| `EqIssuedGr%3Y` |  | Three Year Annualized Growth |
| `EqIssuedGr%5Y` |  | Five Year Annualized Growth |
| `EqIssuedGr%10Y` |  | Ten Year Annualized Growth |
| `EqIssuedRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EqIssuedRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EqIssuedRegEstANN` |  | Ten Year Regression Estimate |
| `EqIssuedRegEstTTM` |  | Five Year Regression Estimate |
| `EqIssuedRegGr%ANN` |  | Ten Year Regression Estimate |
| `EqIssuedRegGr%TTM` |  | Five Year Regression Growth |
| `EqIssuedPSQ` |  | Quarterly Per Share |
| `EqIssuedPSA` |  | Annual Per Share |
| `EqIssued%SalesQ` |  | % of Quarterly Sales |
| `EqIssued%SalesA` |  | % of Annual Sales |
| `EqIssued%AssetsQ` |  | % of Quarterly Assets |
| `EqIssued%AssetsA` |  | % of Annual Assets |
| `EqIssued3YAvg` |  | Three Year Average |
| `EqIssued5YAvg` |  | Five Year Average |


#### Equity Purchased

Cash outflow from equity repurchases.

| Factor | Params | Variant |
|--------|--------|---------|
| `EqPurch()` | offset, type[, NAHandling] |  |
| `EqPurchQ` |  | Latest Quarter |
| `EqPurchPQ` |  | Previous Quarter |
| `EqPurchPYQ` |  | Previous Quarter 1 Year Ago |
| `EqPurchTTM` |  | Trailing 12 Months |
| `EqPurchPTM` |  | Previous Trailing 12 Months |
| `EqPurchA` |  | Latest Year |
| `EqPurchPY` |  | Previous Year |
| `EqPurchGr%PQ` |  | Q vs Previous Q Growth |
| `EqPurchGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `EqPurchGr%TTM` |  | Trailing Twelve Months Growth |
| `EqPurchGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `EqPurchGr%A` |  | Growth Annual |
| `EqPurchGr%3Y` |  | Three Year Annualized Growth |
| `EqPurchGr%5Y` |  | Five Year Annualized Growth |
| `EqPurchGr%10Y` |  | Ten Year Annualized Growth |
| `EqPurchRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `EqPurchRSD%TTM` |  | Five Year Relative Standard Deviation |
| `EqPurchRegEstANN` |  | Ten Year Regression Estimate |
| `EqPurchRegEstTTM` |  | Five Year Regression Estimate |
| `EqPurchRegGr%ANN` |  | Ten Year Regression Estimate |
| `EqPurchRegGr%TTM` |  | Five Year Regression Growth |
| `EqPurchPSQ` |  | Quarterly Per Share |
| `EqPurchPSA` |  | Annual Per Share |
| `EqPurch%SalesQ` |  | % of Quarterly Sales |
| `EqPurch%SalesA` |  | % of Annual Sales |
| `EqPurch%AssetsQ` |  | % of Quarterly Assets |
| `EqPurch%AssetsA` |  | % of Annual Assets |
| `EqPurch3YAvg` |  | Three Year Average |
| `EqPurch5YAvg` |  | Five Year Average |


#### Long Term Debt Issued

Cash inflow from issuing debt with maturity over 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLTIssued()` | offset, type[, NAHandling] |  |
| `DbtLTIssuedQ` |  | Latest Quarter |
| `DbtLTIssuedPQ` |  | Previous Quarter |
| `DbtLTIssuedPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLTIssuedTTM` |  | Trailing 12 Months |
| `DbtLTIssuedPTM` |  | Previous Trailing 12 Months |
| `DbtLTIssuedA` |  | Latest Year |
| `DbtLTIssuedPY` |  | Previous Year |
| `DbtLTIssuedGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLTIssuedGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLTIssuedGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLTIssuedGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLTIssuedGr%A` |  | Growth Annual |
| `DbtLTIssuedGr%3Y` |  | Three Year Annualized Growth |
| `DbtLTIssuedGr%5Y` |  | Five Year Annualized Growth |
| `DbtLTIssuedGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLTIssuedRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLTIssuedRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLTIssuedRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLTIssuedRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLTIssuedRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLTIssuedRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLTIssuedPSQ` |  | Quarterly Per Share |
| `DbtLTIssuedPSA` |  | Annual Per Share |
| `DbtLTIssued%SalesQ` |  | % of Quarterly Sales |
| `DbtLTIssued%SalesA` |  | % of Annual Sales |
| `DbtLTIssued%AssetsQ` |  | % of Quarterly Assets |
| `DbtLTIssued%AssetsA` |  | % of Annual Assets |
| `DbtLTIssued3YAvg` |  | Three Year Average |
| `DbtLTIssued5YAvg` |  | Five Year Average |


#### Long Term Debt Reduced

Cash outflow from retiring debt with maturity over 12 months.

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLTReduced()` | offset, type[, NAHandling] |  |
| `DbtLTReducedQ` |  | Latest Quarter |
| `DbtLTReducedPQ` |  | Previous Quarter |
| `DbtLTReducedPYQ` |  | Previous Quarter 1 Year Ago |
| `DbtLTReducedTTM` |  | Trailing 12 Months |
| `DbtLTReducedPTM` |  | Previous Trailing 12 Months |
| `DbtLTReducedA` |  | Latest Year |
| `DbtLTReducedPY` |  | Previous Year |
| `DbtLTReducedGr%PQ` |  | Q vs Previous Q Growth |
| `DbtLTReducedGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `DbtLTReducedGr%TTM` |  | Trailing Twelve Months Growth |
| `DbtLTReducedGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `DbtLTReducedGr%A` |  | Growth Annual |
| `DbtLTReducedGr%3Y` |  | Three Year Annualized Growth |
| `DbtLTReducedGr%5Y` |  | Five Year Annualized Growth |
| `DbtLTReducedGr%10Y` |  | Ten Year Annualized Growth |
| `DbtLTReducedRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `DbtLTReducedRSD%TTM` |  | Five Year Relative Standard Deviation |
| `DbtLTReducedRegEstANN` |  | Ten Year Regression Estimate |
| `DbtLTReducedRegEstTTM` |  | Five Year Regression Estimate |
| `DbtLTReducedRegGr%ANN` |  | Ten Year Regression Estimate |
| `DbtLTReducedRegGr%TTM` |  | Five Year Regression Growth |
| `DbtLTReducedPSQ` |  | Quarterly Per Share |
| `DbtLTReducedPSA` |  | Annual Per Share |
| `DbtLTReduced%SalesQ` |  | % of Quarterly Sales |
| `DbtLTReduced%SalesA` |  | % of Annual Sales |
| `DbtLTReduced%AssetsQ` |  | % of Quarterly Assets |
| `DbtLTReduced%AssetsA` |  | % of Annual Assets |
| `DbtLTReduced3YAvg` |  | Three Year Average |
| `DbtLTReduced5YAvg` |  | Five Year Average |


### Summary

Cash flow lines that do not fit into the three general activities, such as net flow of cash.

#### Cash Flow

Income After Taxes - Preferred Dividends + Depreciation & Amortization

| Factor | Params | Variant |
|--------|--------|---------|
| `CashFl()` | offset, type[, NAHandling] |  |
| `CashFlQ` |  | Latest Quarter |
| `CashFlPQ` |  | Previous Quarter |
| `CashFlPYQ` |  | Previous Quarter 1 Year Ago |
| `CashFlTTM` |  | Trailing 12 Months |
| `CashFlPTM` |  | Previous Trailing 12 Months |
| `CashFlA` |  | Latest Year |
| `CashFlPY` |  | Previous Year |
| `CashFlGr%PQ` |  | Q vs Previous Q Growth |
| `CashFlGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `CashFlGr%TTM` |  | Trailing Twelve Months Growth |
| `CashFlGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `CashFlGr%A` |  | Growth Annual |
| `CashFlGr%3Y` |  | Three Year Annualized Growth |
| `CashFlGr%5Y` |  | Five Year Annualized Growth |
| `CashFlGr%10Y` |  | Ten Year Annualized Growth |
| `CashFlRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `CashFlRSD%TTM` |  | Five Year Relative Standard Deviation |
| `CashFlRegEstANN` |  | Ten Year Regression Estimate |
| `CashFlRegEstTTM` |  | Five Year Regression Estimate |
| `CashFlRegGr%ANN` |  | Ten Year Regression Estimate |
| `CashFlRegGr%TTM` |  | Five Year Regression Growth |
| `CashFlPSQ` |  | Quarterly Per Share |
| `CashFlPSA` |  | Annual Per Share |
| `CashFl%SalesQ` |  | % of Quarterly Sales |
| `CashFl%SalesA` |  | % of Annual Sales |
| `CashFl%AssetsQ` |  | % of Quarterly Assets |
| `CashFl%AssetsA` |  | % of Annual Assets |
| `CashFl3YAvg` |  | Three Year Average |
| `CashFl5YAvg` |  | Five Year Average |


#### Free Cash Flow

Cash generated after accounting for operational support and capital asset maintenance.

| Factor | Params | Variant |
|--------|--------|---------|
| `FCF()` | offset, type[, NAHandling] |  |
| `FCFQ` |  | Latest Quarter |
| `FCFPQ` |  | Previous Quarter |
| `FCFPYQ` |  | Previous Quarter 1 Year Ago |
| `FCFTTM` |  | Trailing 12 Months |
| `FCFPTM` |  | Previous Trailing 12 Months |
| `FCFA` |  | Latest Year |
| `FCFPY` |  | Previous Year |
| `FCFGr%PQ` |  | Q vs Previous Q Growth |
| `FCFGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `FCFGr%TTM` |  | Trailing Twelve Months Growth |
| `FCFGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `FCFGr%A` |  | Growth Annual |
| `FCFGr%3Y` |  | Three Year Annualized Growth |
| `FCFGr%5Y` |  | Five Year Annualized Growth |
| `FCFGr%10Y` |  | Ten Year Annualized Growth |
| `FCFRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `FCFRSD%TTM` |  | Five Year Relative Standard Deviation |
| `FCFRegEstANN` |  | Ten Year Regression Estimate |
| `FCFRegEstTTM` |  | Five Year Regression Estimate |
| `FCFRegGr%ANN` |  | Ten Year Regression Estimate |
| `FCFRegGr%TTM` |  | Five Year Regression Growth |
| `FCFPSQ` |  | Quarterly Per Share |
| `FCFPSA` |  | Annual Per Share |
| `FCF%SalesQ` |  | % of Quarterly Sales |
| `FCF%SalesA` |  | % of Annual Sales |
| `FCF%AssetsQ` |  | % of Quarterly Assets |
| `FCF%AssetsA` |  | % of Annual Assets |
| `FCF3YAvg` |  | Three Year Average |
| `FCF5YAvg` |  | Five Year Average |


#### Net Change to Cash Position

Total change in cash for the period.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetChgCash()` | offset, type[, NAHandling] |  |
| `NetChgCashQ` |  | Latest Quarter |
| `NetChgCashPQ` |  | Previous Quarter |
| `NetChgCashPYQ` |  | Previous Quarter 1 Year Ago |
| `NetChgCashTTM` |  | Trailing 12 Months |
| `NetChgCashPTM` |  | Previous Trailing 12 Months |
| `NetChgCashA` |  | Latest Year |
| `NetChgCashPY` |  | Previous Year |
| `NetChgCashGr%PQ` |  | Q vs Previous Q Growth |
| `NetChgCashGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetChgCashGr%TTM` |  | Trailing Twelve Months Growth |
| `NetChgCashGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetChgCashGr%A` |  | Growth Annual |
| `NetChgCashGr%3Y` |  | Three Year Annualized Growth |
| `NetChgCashGr%5Y` |  | Five Year Annualized Growth |
| `NetChgCashGr%10Y` |  | Ten Year Annualized Growth |
| `NetChgCashRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetChgCashRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetChgCashRegEstANN` |  | Ten Year Regression Estimate |
| `NetChgCashRegEstTTM` |  | Five Year Regression Estimate |
| `NetChgCashRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetChgCashRegGr%TTM` |  | Five Year Regression Growth |
| `NetChgCashPSQ` |  | Quarterly Per Share |
| `NetChgCashPSA` |  | Annual Per Share |
| `NetChgCash%SalesQ` |  | % of Quarterly Sales |
| `NetChgCash%SalesA` |  | % of Annual Sales |
| `NetChgCash%AssetsQ` |  | % of Quarterly Assets |
| `NetChgCash%AssetsA` |  | % of Annual Assets |
| `NetChgCash3YAvg` |  | Three Year Average |
| `NetChgCash5YAvg` |  | Five Year Average |


#### Net Free Cash Flow

Cash generated after supporting operations, maintaining capital assets, and paying dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `NetFCF()` | offset, type |  |
| `NetFCFQ` |  | Latest Quarter |
| `NetFCFPQ` |  | Previous Quarter |
| `NetFCFPYQ` |  | Previous Quarter 1 Year Ago |
| `NetFCFTTM` |  | Trailing 12 Months |
| `NetFCFPTM` |  | Previous Trailing 12 Months |
| `NetFCFA` |  | Latest Year |
| `NetFCFPY` |  | Previous Year |
| `NetFCFGr%PQ` |  | Q vs Previous Q Growth |
| `NetFCFGr%PYQ` |  | Q vs 1 year ago Q Growth |
| `NetFCFGr%TTM` |  | Trailing Twelve Months Growth |
| `NetFCFGr%PQTTM` |  | Trailing Twelve Months Growth 1Q Ago |
| `NetFCFGr%A` |  | Growth Annual |
| `NetFCFGr%3Y` |  | Three Year Annualized Growth |
| `NetFCFGr%5Y` |  | Five Year Annualized Growth |
| `NetFCFGr%10Y` |  | Ten Year Annualized Growth |
| `NetFCFRSD%ANN` |  | Ten Year Relative Standard Deviation |
| `NetFCFRSD%TTM` |  | Five Year Relative Standard Deviation |
| `NetFCFRegEstANN` |  | Ten Year Regression Estimate |
| `NetFCFRegEstTTM` |  | Five Year Regression Estimate |
| `NetFCFRegGr%ANN` |  | Ten Year Regression Estimate |
| `NetFCFRegGr%TTM` |  | Five Year Regression Growth |
| `NetFCFPSQ` |  | Quarterly Per Share |
| `NetFCFPSA` |  | Annual Per Share |
| `NetFCF%SalesQ` |  | % of Quarterly Sales |
| `NetFCF%SalesA` |  | % of Annual Sales |
| `NetFCF%AssetsQ` |  | % of Quarterly Assets |
| `NetFCF%AssetsA` |  | % of Annual Assets |
| `NetFCF3YAvg` |  | Three Year Average |
| `NetFCF5YAvg` |  | Five Year Average |

