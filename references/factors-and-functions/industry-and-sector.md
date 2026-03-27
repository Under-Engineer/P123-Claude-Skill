# Industry & Sector

Industry and Sector functions

## Classification

Industry, sector and universe classifications.

### Industry

Which industry the stock belongs to. For example, to screen for stocks in the leisure products industry use: Industry=LEISURE

| Factor | Params | Variant |
|--------|--------|---------|
| `Industry` |  |  |


### Industry Code

Industry Code. See Full Description for a complete list of codes

| Factor | Params | Variant |
|--------|--------|---------|
| `IndCode` |  |  |


### Industry Description

See Full Description for a complete list of names

| Factor | Params | Variant |
|--------|--------|---------|
| `IndDescr` |  |  |


### Revere Industry Classification (RBICS)

Evaluates to TRUE if any combination of RBICS Sector, Sub-sector, Industry, and Sub-industry matches.

For example, RBICS(25, 401515) returns stocks in *either* Sector ENERGY or Industry DELIVERY. You can also use our mnemonics: RBICS(ENERGY, DELIVERY)

| Factor | Params | Variant |
|--------|--------|---------|
| `RBICS()` | rcode, rcode, rcode, ... |  |


### Sector

Which sector the stock belongs to. For example, to screen for stocks in the technology sector use: Sector=TECH

| Factor | Params | Variant |
|--------|--------|---------|
| `Sector` |  |  |


### Sector Code

Sector Code. See Full Description for a complete list of codes

| Factor | Params | Variant |
|--------|--------|---------|
| `SectorCode` |  |  |


### Sector Description

Sector Description. See Full Description for a complete list of names

| Factor | Params | Variant |
|--------|--------|---------|
| `SectorDescr` |  |  |


### SubIndustry

Which sub-industry the stock belongs to. For example, to screen for stocks in the diversified REITs sub-industry use: SubIndustry=REITDIV

| Factor | Params | Variant |
|--------|--------|---------|
| `SubIndustry` |  |  |


### SubIndustry Code

See Full Description for a complete list of codes

| Factor | Params | Variant |
|--------|--------|---------|
| `SubIndCode` |  |  |


### SubIndustry Description

See Full Description for a complete list of names

| Factor | Params | Variant |
|--------|--------|---------|
| `SubIndDescr` |  |  |


### SubSector

Which sub-sector the stock belongs to.

| Factor | Params | Variant |
|--------|--------|---------|
| `SubSector` |  |  |


### SubSector Code

SubSector Code. See Full Description for a complete list of codes

| Factor | Params | Variant |
|--------|--------|---------|
| `SubSectorCode` |  |  |


### SubSector Description

SubSector Description. See Full Description for a complete list of names

| Factor | Params | Variant |
|--------|--------|---------|
| `SubSectorDescr` |  |  |


## Ind Aggregate Factors

Contains precalculated industry factors. The factors that end with Ind are calculated using the Aggregate cross-sectional function. See Full description for more details

### Descriptive

Number of constituents in a given industry.

#### Number of Constituents

Number of constituents in the industry

| Factor | Params | Variant |
|--------|--------|---------|
| `NoConst` |  |  |


### Dividend

Aggregated dividend yield.

#### Yield, Industry

Dividend Yield Industry, 5 Year Average (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `Yield5YAvgInd` |  | 5 Years |
| `YieldInd` |  |  |


### Efficiency

Aggregated turnover and per-employee ratios.

#### Asset Turnover, Industry

Asset Turnover Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `AstTurnTTMInd` |  | Trailing Twelve Months |


#### Income per Employee, Industry

Income Per Employee Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `IncPerEmpTTMInd` |  | Trailing 12 Months |


#### Inventory Turnover, Industry

Inventory Turnover Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `InvTurnTTMInd` |  | Trailing 12 Months |


#### Receivable Turnover, Industry

Receivables Turnover Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `RecTurnTTMInd` |  | Trailing 12 Months |


#### Sales per Employee, Industry

Sales Per Employee Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `SalesPerEmpTTMInd` |  | Trailing Twelve Months |


### Estimates

Aggregated mean estimate revisions for industries.

#### Estimate Revision Direction

Ratio ranging from -1 to +1 indicating the direction of revisions for the stock's industry. The extreme values 1 and -1 would indicate that every analyst's CurrY estimate in the industry have been revised upward and downward respectively in the past 4 Weeks.

| Factor | Params | Variant |
|--------|--------|---------|
| `CurrYRevRatio4W` |  | Current Year |
| `NextYRevRatio4W` |  | Next Year |


### Financial Strength

Aggregated ratios relating to quality, including payout and debt ratios.

#### Current Ratio, Industry

Current Ratio Industry, Quarterly

| Factor | Params | Variant |
|--------|--------|---------|
| `CurRatioQInd` |  | Latest Quarter |


#### Interest Coverage, Industry

Interest Coverage Industry, TTM


| Factor | Params | Variant |
|--------|--------|---------|
| `IntCovTTMInd` |  | Trailing 12 Months |


#### Long Term Debt To Total Equity, Industry

Long Term Debt To Total Equity Industry, Quarterly

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtLT2EqQInd` |  | Latest Quarter |


#### Payout Ratio, Industry

Payout Ratio Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `PayRatio5YAvgInd` |  | 5 Years |
| `PayRatio5YInd` |  | 5 Years |
| `PayRatioTTMInd` |  | Trailing 12 Months |


#### Quick Ratio, Industry

Quick Ratio Industry, Quarterly

| Factor | Params | Variant |
|--------|--------|---------|
| `QuickRatioQInd` |  | Latest Quarter |


#### Retention Rate, Industry

Retention Rate Industry, TTM (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `Retn%TTMInd` |  | Trailing 12 Months |


#### Total Debt To Total Equity, Industry

Total Debt To Total Equity Industry, Quarterly

| Factor | Params | Variant |
|--------|--------|---------|
| `DbtTot2EqQInd` |  | Latest Quarter |


### Growth Rates

Aggregated industrial growth rates.

#### Industry Growth

Capital Spending Industry, 5 Year Growth Rate (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `CapSp5YCGr%Ind` |  | 5 Years |
| `Div%ChgAInd` |  | Latest Year |
| `Div3YCGr%Ind` |  | 3 Years |
| `Div5YCGr%Ind` |  | 5 Years |
| `EPSExclXorGr%3YInd` |  | 3 Years |
| `EPSExclXorGr%5YInd` |  | 5 Years |
| `EPSExclXorGr%AInd` |  | Latest Year |
| `EPSExclXorGr%PYQInd` |  | Latest Quarter vs 1 Year Ago |
| `EPSExclXorGr%TTMInd` |  | Trailing 12 Months |
| `SalesGr%3YInd` |  | 3 Years |
| `SalesGr%5YInd` |  | 5 Years |
| `SalesGr%AInd` |  | Latest Year |
| `SalesGr%PYQInd` |  | Latest Quarter vs 1 Year Ago |
| `SalesGr%TTMInd` |  | Trailing 12 Months |


### Institutional Ownership

Aggregated per industry institutional ownership rates.

#### Institutional % Owned, Industry

Institutional Percent Owned Industry, (%) average

| Factor | Params | Variant |
|--------|--------|---------|
| `Inst%OwnInd` |  |  |


### Price & Volume

Aggregated industrial price changes.

#### Price Percent Change, Industry

13 Week Price Percent Change Industry (%)

NOTE: See Full Description for important information

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr13W%ChgInd` |  | 13 Weeks |
| `Pr26W%ChgInd` |  | 26 Weeks |
| `Pr4W%ChgInd` |  | 4 Weeks |
| `Pr52W%ChgInd` |  | 52 Weeks |


#### Relative Price Percent Change, Industry

Relative Price Percent Change Industry, 13 Weeks (%)

NOTE: Not the same as our Industry & Sector which is cap-weighted

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr13WRel%ChgInd` |  | 13 Weeks |
| `Pr26WRel%ChgInd` |  | 26 Weeks |
| `Pr4WRel%ChgInd` |  | 4 Weeks |
| `Pr52WRel%ChgInd` |  | 52 Weeks |


### Profitability

Aggregated margins and management efficiency ratios.

#### EBITDA Margin, Industry

EBITDA Margin Industry, 5 year average (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAMgn%5YAvgInd` |  | 5 Years |
| `EBITDAMgn%5YInd` |  | 5 Years |


#### Gross Profit Margin, Industry

Gross Margin Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `GMgn%5YAvgInd` |  | 5 Years |
| `GMgn%5YInd` |  | 5 Years |
| `GMgn%TTMInd` |  | Trailing 12 Months |


#### Net Profit Margin, Industry

Net Profit Margin Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `NPMgn%5YAvgInd` |  | 5 Years |
| `NPMgn%5YInd` |  | 5 Years |
| `NPMgn%TTMInd` |  | Trailing 12 Months |


#### Pretax Margin, Industry

Pretax Margin Industry, 5 Year Average (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `PTMgn%5YAvgInd` |  | 5 Years |
| `PTMgn%5YInd` |  | 5 Years |
| `PTMgn%TTMInd` |  | Trailing 12 Months |


#### Return On Assets, Industry

Return on Average Assets Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `ROA%5YAvgInd` |  | 5 Years |
| `ROA%TTMInd` |  | Trailing 12 Months |


#### Return On Equity, Industry

Return on Average Common Equity Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `ROE%5YAvgInd` |  | 5 Years |
| `ROE%TTMInd` |  | Trailing 12 Months |


#### Return On Investment, Industry

Return on Investment Industry, 5 Year Average (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `ROI%5YAvgInd` |  | 5 Years |
| `ROI%TTMInd` |  | Trailing 12 Months |


#### Tax Rate, Industry

Tax Rate Industry, Effective, TTM (%)


| Factor | Params | Variant |
|--------|--------|---------|
| `TaxRate%TTMInd` |  | Trailing Twelve Months |


#### Operating Margin, Industry

Operating Margin Industry, TTM (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `OpMgn%TTMInd` |  | Trailing 12 Months |
| `OpMgn%5YAvgInd` |  | 5 Years |
| `OpMgn%5YInd` |  | 5 Years |


### Valuation

Per industry aggregates of prices to fundamental line items.

#### Price To Book, Industry

Price to Book Ratio Industry, Quarterly


| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2BookQInd` |  | Latest Quarter |


#### Price To Cash Flow, Industry

Price to Cash Flow Per Share Ratio Industry, TTM

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2CashFlTTMInd` |  | Trailing 12 Months |


#### Price To Earnings (PE), Industry

Price To Earnings Ratio Industry, Excluding Extraordinary Items, TTM

| Factor | Params | Variant |
|--------|--------|---------|
| `PEExclXorTTMInd` |  | Trailing 12 Months |
| `PEHighInd` |  | 5 Years |
| `PELowInd` |  | 5 Years |


#### Price To Free Cash Flow, Industry

Price To Free Cash Flow Per Share Ratio Industry, TTM

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2FrCashFlTTMInd` |  | Trailing 12 Months |


#### Price To Sales, Industry

Price To Sales Next Twelve Months

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2SalesNTMInd` |  | Trailing Twelve Months |
| `Pr2SalesTTMInd` |  | Trailing Twelve Months |


#### Price To Tangible Book, Industry

Price to Tangible Book Ratio Industry, Quarterly


| Factor | Params | Variant |
|--------|--------|---------|
| `Pr2TanBkQInd` |  | Latest Quarter |


### Valuation Projected

#### PEG Ratio, Industry

Projected Price/Earnings to Long Term Growth Rate Industry

| Factor | Params | Variant |
|--------|--------|---------|
| `PEGLTInd` |  | Long Term Growth |
| `PEGSTInd` |  | Next Year Growth |


#### Price To Earnings (PE) Projected, Industry

Next Year Projected P/E Ratio Industry

| Factor | Params | Variant |
|--------|--------|---------|
| `ProjPENextFYInd` |  | Next Fiscal Year |
| `ProjPENTMInd` |  | Next Twelve Months |


### Volatility

Aggregated betas per industry.

#### Beta, Industry

Beta1Y for the industry

| Factor | Params | Variant |
|--------|--------|---------|
| `Beta1YInd` |  | 1 Year |
| `Beta3YInd` |  | 3 Years |
| `Beta5YInd` |  | 5 Years |

