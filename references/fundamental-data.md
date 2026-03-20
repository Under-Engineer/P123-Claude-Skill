# P123 Fundamental Data Reference

All fundamental items follow the same pattern:

```
FunctionName(offset, periodType [, NAHandling])
```
- **offset**: 0=most recent, 1=one period back, ... (0-20 for QTR, 0-10 for ANN)
- **periodType**: `QTR` (quarterly), `ANN` (annual), `TTM` (trailing 12 months)
- **NAHandling**: `FALLBACK` (default), `KEEPNA`, `ZERONA`

Each item also generates pre-built factors (no parentheses): see Pattern Guide at bottom.

---

## Balance Sheet — Current Assets

| Function | Description |
|----------|-------------|
| `Cash(offset, type)` | Cash only |
| `CashEquiv(offset, type)` | Cash and equivalents (cash + short-term investments) |
| `InvstST(offset, type)` | Short-term investments (not included in CashEquiv on some companies) |
| `Recvbl(offset, type)` | Accounts receivable (net of allowances) |
| `Inventory(offset, type)` | Inventories |
| `AstCurOther(offset, type)` | Other current assets |
| `AstCur(offset, type)` | **Total current assets** |
| `WorkCap(offset, type)` | Working capital (AstCur − LiabCur) |

## Balance Sheet — Non-Current Assets

| Function | Description |
|----------|-------------|
| `GrossPlant(offset, type)` | Gross property, plant & equipment |
| `AccumDep(offset, type)` | Accumulated depreciation |
| `NetPlant(offset, type)` | Net PP&E (GrossPlant − AccumDep) |
| `Goodwill(offset, type)` | Goodwill |
| `AstIntan(offset, type)` | Intangible assets |
| `IntanOther(offset, type)` | Other intangibles |
| `InvstEq(offset, type)` | Equity investments |
| `InvstAdvOther(offset, type)` | Investments and advances, other |
| `AstNonCurOther(offset, type)` | Other non-current assets |
| `AstTot(offset, type)` | **Total assets** |

## Balance Sheet — Current Liabilities

| Function | Description |
|----------|-------------|
| `Payables(offset, type)` | Accounts payable |
| `DbtST(offset, type)` | Short-term debt (due within 12 months) |
| `TxPayable(offset, type)` | Taxes payable |
| `LiabCurOther(offset, type)` | Other current liabilities |
| `LiabCur(offset, type)` | **Total current liabilities** |

## Balance Sheet — Non-Current Liabilities

| Function | Description |
|----------|-------------|
| `DbtLT(offset, type)` | Long-term debt |
| `DbtTot(offset, type)` | Total debt (short-term + long-term) |
| `CapLease(offset, type)` | Capital lease obligations |
| `TxDfdIC(offset, type)` | Deferred taxes and investment credits |
| `LiabNonCurOther(offset, type)` | Other non-current liabilities |
| `LiabTot(offset, type)` | **Total liabilities** |

## Balance Sheet — Shareholders' Equity

| Function | Description |
|----------|-------------|
| `ComEq(offset, type)` | Common equity |
| `BookVal(offset, type)` | Book value |
| `RetainedEarn(offset, type)` | Retained earnings |
| `PfdEquity(offset, type)` | Preferred equity |
| `CapSurplus(offset, type)` | Capital surplus (additional paid-in capital) |
| `NonControlInt(offset, type)` | Non-controlling interest (total) |
| `NonControlIntNonRed(offset, type)` | Non-controlling interest, non-redeemable |
| `NonControlIntRed(offset, type)` | Non-controlling interest, redeemable |
| `EqTot(offset, type)` | **Shareholder's equity total** |
| `TanBV(offset, type)` | Tangible book value (net tangible assets) |

## Balance Sheet — Shares

| Function | Description |
|----------|-------------|
| `Shares(offset, type)` | Common shares outstanding |
| `SharesFD(offset, type)` | Common shares fully diluted |
| `SharesCur(barsAgo)` | Common shares most recent (takes bars, not offset/type) |

---

## Income Statement

| Function | Description |
|----------|-------------|
| `Sales(offset, type)` | **Revenue / Net sales** |
| `SalesIntl(offset, type)` | International sales |
| `CostG(offset, type)` | Cost of goods sold |
| `CostG_GAAP(offset, type)` | Cost of goods sold (GAAP) |
| `GrossProfit(offset, type)` | Gross profit |
| `GrossProfit_GAAP(offset, type)` | Gross profit (GAAP) |
| `SGandA(offset, type)` | Selling, general & administrative expense |
| `SGandA_GAAP(offset, type)` | SG&A (GAAP) |
| `RandD(offset, type)` | Research & development expense |
| `OpInc(offset, type)` | **Operating income** |
| `OpIncBDepr(offset, type)` | Operating income before depreciation |
| `OpIncAftDepr(offset, type)` | Operating income after depreciation |
| `EBIT(offset, type)` | Earnings before interest and taxes |
| `EBITDA(offset, type)` | EBITDA |
| `IntExp(offset, type)` | Interest expense |
| `IntInc(offset, type)` | Interest income |
| `ExpNonOp(offset, type)` | Non-operating expenses |
| `IncBTax(offset, type)` | **Income before taxes (pre-tax income)** |
| `IncTaxExp(offset, type)` | Income tax expense |
| `IncAftTax(offset, type)` | **Income after taxes** |
| `IAC(offset, type)` | Income available to common |
| `NetIncBXor(offset, type)` | Net income before extraordinary items |
| `NetIncBXorNonC(offset, type)` | Net income before xor and non-controlling interest |
| `IncBXorForCom(offset, type)` | Income before xor items available for common |
| `IncBXorAdjCSE(offset, type)` | Income before xor items adjusted for common stock equivalents |
| `EPSExclXor(offset, type)` | **EPS excluding extraordinary items** |
| `EPSInclXor(offset, type)` | EPS including extraordinary items |
| `DivPS(offset, type)` | Dividends per share |
| `DepAmort(offset, type)` | Depreciation & amortization |
| `Amort(offset, type)` | Amortization of intangibles |
| `FundsFromOp(offset, type)` | Funds from operations (REITs) |
| `StkOptExp(offset, type)` | Stock option compensation expense |
| `PfdDiv(offset, type)` | Preferred dividends paid |
| `SpcItems(offset, type)` | Special items |
| `Impair(offset, type)` | Impairment charges |

---

## Cash Flow Statement

### Operating
| Function | Description |
|----------|-------------|
| `OperCashFl(offset, type)` | **Operating cash flow** |
| `NetIncCFStmt(offset, type)` | Net income (cash flow statement) |
| `DepAmortCF(offset, type)` | Depreciation & amortization (cash flow line) |
| `TxDfd(offset, type)` | Deferred taxes |
| `StkOptCF(offset, type)` | Stock option compensation (cash flow line) |
| `RecvblChg(offset, type)` | Change in accounts receivables |
| `InvtyChg(offset, type)` | Change in inventories |
| `PayablesChg(offset, type)` | Change in accounts payable |
| `AccruedExp(offset, type)` | Change in accrued liabilities (accrued expenses) |
| `TxAcrudChg(offset, type)` | Change in accrued income taxes |
| `OtherWCChg(offset, type)` | Change in other working capital lines |

### Investing
| Function | Description |
|----------|-------------|
| `CapEx(offset, type)` | **Capital expenditures** |
| `CashFrInvest(offset, type)` | Cash from investing |
| `Acquis(offset, type)` | Acquisitions |
| `Divest(offset, type)` | Divestitures |
| `InvstOther(offset, type)` | Other investing cash flow |

### Financing
| Function | Description |
|----------|-------------|
| `CashFrFin(offset, type)` | Cash from financing |
| `ChangeDebt(offset, type)` | Change in debt (net) |
| `ChangeEq(offset, type)` | Change in equity (net) |
| `DbtLTIssued(offset, type)` | Long-term debt issued |
| `DbtLTReduced(offset, type)` | Long-term debt reduced |
| `EqIssued(offset, type)` | Equity issued |
| `EqPurch(offset, type)` | Equity purchased (buybacks) |
| `DivPaid(offset, type)` | Dividends paid (total) |

### Summary
| Function | Description |
|----------|-------------|
| `CashFl(offset, type)` | Total cash flow |
| `FCF(offset, type)` | **Free cash flow** (OperCashFl − CapEx) |
| `NetFCF(offset, type)` | Net free cash flow (OperCashFl − CapEx − DivPaid) |
| `NetChgCash(offset, type)` | Net change in cash position |

---

## Key Pre-Built Ratios & Statistics

### Valuation

| Factor | Function | Description |
|--------|----------|-------------|
| `PEExclXorTTM` | `PEExclXor(offset, type)` | **P/E excluding extraordinary items** |
| `PEInclXorTTM` | `PEInclXor(offset, type)` | P/E including extraordinary items |
| `PEInclRDTTM` | `PEInclRD(offset, type)` | Innovation P/E (incl R&D capitalized) |
| `Pr2BookQ` | `Pr2Book(offset, type)` | **Price to book** |
| `Pr2SalesTTM` | `Pr2Sales(offset, type)` | **Price to sales** |
| `Pr2CashFlTTM` | `Pr2CashFl(offset, type)` | Price to cash flow |
| `Pr2FrCashFlTTM` | `Pr2FrCashFl(offset, type)` | **Price to free cash flow** |
| `Pr2NetFrCashFlTTM` | `Pr2NetFrCashFl(offset, type)` | Price to net free cash flow |
| `Pr2TanBkQ` | `Pr2TanBk(offset, type)` | Price to tangible book value |
| `EV2EBITDATTM` | `EV2EBITDA(offset, type)` | **EV/EBITDA** |
| `EV2SalesTTM` | `EV2Sales(offset, type)` | EV/Sales |

### Yield

| Factor | Description |
|--------|-------------|
| `DivYield%TTM` | **Dividend yield** |
| `EarnYield%TTM` | Earnings yield (inverse of PE) |
| `ShrYield%TTM` | Shareholder yield (dividends + buybacks) |
| `EBITDAYield%TTM` | EBITDA yield |
| `FCFYield%TTM` | Free cash flow yield |
| `OCFYield%TTM` | Operating cash flow yield |
| `OpIncYield%TTM` | Operating income yield |

### Margins

| Factor | Function | Description |
|--------|----------|-------------|
| `GMgn%TTM` | `GMgn%(offset, type)` | **Gross margin** |
| `GMgn%_GAAPTTM` | `GMgn%_GAAP(offset, type)` | Gross margin (GAAP) |
| `OpMgn%TTM` | `OpMgn%(offset, type)` | **Operating margin** |
| `NPMgn%TTM` | `NPMgn%(offset, type)` | **Net profit margin** |
| `PTMgn%TTM` | `PTMgn%(offset, type)` | Pre-tax margin |
| `EBITDAMgn%TTM` | `EBITDAMgn%(offset, type)` | EBITDA margin |
| `FCFLMgn%TTM` | `FCFLMgn%(offset, type)` | Free cash flow margin |
| `NetFCFLMgn%TTM` | `NetFCFLMgn%(offset, type)` | Net free cash flow margin |
| `SGA2Sales%TTM` | `SGA2Sales%(offset, type)` | SG&A as % of sales |

### Profitability

| Factor | Function | Description |
|--------|----------|-------------|
| `ROE%TTM` | `ROE%(offset, type)` | **Return on equity** |
| `ROA%TTM` | `ROA%(offset, type)` | **Return on assets** |
| `ROI%TTM` | `ROI%(offset, type)` | Return on investment |

### Per Share Ratios

| Factor | Function | Description |
|--------|----------|-------------|
| `BVPSTTM` | `BVPS(offset, type)` | Book value per share |
| `CashPSTTM` | `CashPS(offset, type)` | Cash per share |
| `SalesPSTTM` | `SalesPS(offset, type)` | Sales per share |
| `CashFlPSTTM` | `CashFlPS(offset, type)` | Cash flow per share |
| `FCFPSTTM` | `FCFPS(offset, type)` | Free cash flow per share |
| `NetFCFPSTTM` | `NetFCFPS(offset, type)` | Net free cash flow per share |
| `OCFPSTTM` | `OCFPS(offset, type)` | Operating cash flow per share |
| `OpIncPSTTM` | `OpIncPS(offset, type)` | Operating income per share |
| `CapExPSTTM` | `CapExPS(offset, type)` | Capital expenditures per share |
| `EBITDAPSTTM` | `EBITDAPS(offset, type)` | EBITDA per share |

### Efficiency

| Factor | Function | Description |
|--------|----------|-------------|
| `AstTurnTTM` | `AstTurn(offset, type)` | Asset turnover |
| `InvTurnTTM` | `InvTurn(offset, type)` | Inventory turnover |
| `RecTurnTTM` | `RecTurn(offset, type)` | Receivables turnover |
| `IncPerEmpTTM` | `IncPerEmp(offset, type)` | Income per employee |
| `SalesPerEmpTTM` | `SalesPerEmp(offset, type)` | Sales per employee |
| `SGA2GPTTM` | `SGA2GP(offset, type)` | SG&A to gross profit |

### Financial Strength

| Factor | Function | Description |
|--------|----------|-------------|
| `CurRatioQ` | `CurRatio(offset, type)` | Current ratio |
| `QuickRatioQ` | `QuickRatio(offset, type)` | Quick ratio |
| `DbtTot2EqQ` | `DbtTot2Eq(offset, type)` | **Total debt to equity** |
| `DbtTot2AstQ` | `DbtTot2Ast(offset, type)` | Total debt to assets |
| `DbtTot2CapQ` | `DbtTot2Cap(offset, type)` | Total debt to capital |
| `DbtLT2EqQ` | `DbtLT2Eq(offset, type)` | Long-term debt to equity |
| `DbtLT2AstQ` | `DbtLT2Ast(offset, type)` | Long-term debt to assets |
| `DbtLT2CapQ` | `DbtLT2Cap(offset, type)` | Long-term debt to capital |
| `IntCovTTM` | `IntCov(offset, type)` | Interest coverage |
| `DbtS2NITTM` | `DbtS2NI(offset, type)` | Debt service to net income |
| `NI2CapExTTM` | `NI2CapEx(offset, type)` | Net income to capital expenditures |
| `PayRatioTTM` | `PayRatio(offset, type)` | Payout ratio |
| `Retn%TTM` | `Retn%(offset, type)` | Retention rate |
| `DepAmort2GPTTM` | `DepAmort2GP(offset, type)` | Depreciation & amort to gross profit |

### Advanced Scores

| Factor | Description |
|--------|-------------|
| `AltmanZ` | Altman Z-score (bankruptcy predictor) |
| `AltmanX1` ... `AltmanX5` | Individual Altman Z components |
| `PiotroskiF` | Piotroski F-score (financial strength, 0-9) |
| `BeneishM` | Beneish M-score (earnings manipulation detector) |

### Other

| Factor | Description |
|--------|-------------|
| `MktCap` | **Market capitalization** |
| `EntVal` | Enterprise value |
| `Float` | Shares float |
| `Beta` | Beta (from `BetaFunc()`) |

### Market / Price

| Factor | Description |
|--------|-------------|
| `AvgDailyTot(N)` | Avg daily dollar volume over N bars |

### Estimates

| Factor | Description |
|--------|-------------|
| `EstEPSCQ` | EPS estimate current quarter |
| `EstEPSNQ` | EPS estimate next quarter |
| `EstEPSCY` | EPS estimate current year |
| `EstEPSNY` | EPS estimate next year |
| `EstEPSGr%NQ` | Estimated EPS growth next quarter |
| `EstEPSGr%NY` | Estimated EPS growth next year |
| `NumEstEPSCQ` | Number of analyst estimates CQ |
| `EPSSurprise%CQ` | EPS surprise % current quarter |
| `SumRevisions` | Sum of EPS revisions |
| `EstSalesCY` | Sales estimate current year |
| `EstSalesNY` | Sales estimate next year |
| `AvgRec` | Average analyst recommendation (1=Strong Buy to 5=Strong Sell) |
| `LTGrRt` | Long-term EPS growth rate estimate |

### Insider & Institutional

| Factor | Description |
|--------|-------------|
| `InsiderBuySell%3Mo` | Insider buy/sell ratio (3 month) |
| `InsiderBuySell%6Mo` | Insider buy/sell ratio (6 month) |
| `InstOwn%` | Institutional ownership % |
| `InstOwnChg%QoQ` | Institutional ownership change QoQ |
| `ShortInt%Float` | Short interest as % of float |
| `ShortInt%ShOut` | Short interest as % of shares outstanding |
| `ShortIntRatio` | Short interest ratio (days to cover) |

---

## Pre-Built Factor Naming Pattern

For any base function `Item`, P123 auto-generates factors:

| Suffix | Meaning | Example |
|--------|---------|---------|
| `Q` | Most recent quarter | `SalesQ` |
| `A` | Most recent annual | `SalesA` |
| `TTM` | Trailing 12 months | `SalesTTM` |
| `PQ` | Previous quarter | `SalesPQ` |
| `PY` | Previous year | `SalesPY` |
| `PYQ` | Previous year same quarter | `SalesPYQ` |
| `PTM` | Previous trailing 12 months | `SalesPTM` |
| `Gr%TTM` | Growth TTM vs prior TTM | `SalesGr%TTM` |
| `Gr%A` | Growth annual vs prior annual | `SalesGr%A` |
| `Gr%PQ` | Growth QoQ | `SalesGr%PQ` |
| `Gr%PYQ` | Growth Q vs prior year Q (YoY) | `SalesGr%PYQ` |
| `Gr%PQTTM` | Growth in TTM vs prior Q TTM | `SalesGr%PQTTM` |
| `Gr%3Y` | 3-year CAGR | `SalesGr%3Y` |
| `Gr%5Y` | 5-year CAGR | `SalesGr%5Y` |
| `Gr%10Y` | 10-year CAGR | `SalesGr%10Y` |
| `PSA` | Per share (annual) | `SalesPSA` |
| `PSQ` | Per share (quarterly) | `SalesPSQ` |
| `%AssetsA` | As % of assets (annual) | `Sales%AssetsA` |
| `%AssetsQ` | As % of assets (quarterly) | `Sales%AssetsQ` |
| `%SalesA` | As % of sales (annual) | `CapEx%SalesA` |
| `%SalesQ` | As % of sales (quarterly) | `CapEx%SalesQ` |
| `3YAvg` | 3-year average | `Sales3YAvg` |
| `5YAvg` | 5-year average | `Sales5YAvg` |
| `RegGr%ANN` | Regression growth (annual) | `SalesRegGr%ANN` |
| `RegGr%TTM` | Regression growth (TTM) | `SalesRegGr%TTM` |
| `RSD%ANN` | Regression residual std dev (annual) | `SalesRSD%ANN` |
| `RSD%TTM` | Regression residual std dev (TTM) | `SalesRSD%TTM` |
| `RegEstANN` | Regression estimate (annual) | `SalesRegEstANN` |
| `RegEstTTM` | Regression estimate (TTM) | `SalesRegEstTTM` |

---

## Company / Classification

| Factor | Description |
|--------|-------------|
| `SectorId` | GICS sector code (10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60) |
| `IndustryId` | GICS industry code (8-digit) |
| `SubIndId` | GICS sub-industry code |
| `ExchCountry("cid")` | Exchange country filter (function) |
| `Country("cid")` | Country of domicile filter (function) |
| `FYEndMonth` | Fiscal year end month (1-12) |
| `NoEmp` | Number of employees |
| `CoName("name")` | Match company name (returns TRUE/FALSE) |
| `Ticker("AAPL")` | Match ticker |
| `FIGI("figi")` | Match FIGI identifier |
| `#APeriods` | Number of historical annual periods available |
| `#QPeriods` | Number of historical quarterly periods available |

**GICS Sectors**: 10=Energy, 15=Materials, 20=Industrials, 25=Consumer Disc, 30=Consumer Staples, 35=Health Care, 40=Financials, 45=Info Tech, 50=Communication, 55=Utilities, 60=Real Estate
