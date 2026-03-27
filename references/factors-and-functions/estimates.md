# Estimates

Data relating to consensus analyst estimates.

## Estimate Functions

Consensus estimate functions

### Consensus Relative Standard Deviation

Relative Standard Deviation of analysts estimates in percentage

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstRSD()` | cons_item [, period, weekAgo] |  |


### Consensus Down

Number of analysts revising estimate down in past 75 days

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstDn()` | cons_item [, period, weekAgo] |  |


### Consensus High

Consensus highest estimate

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstHi()` | cons_item [, period, weekAgo] |  |


### Consensus Low

Consensus lowest estimate

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstLow()` | cons_item [, period, weekAgo] |  |


### Consensus Mean

Average of analyst estimates

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstMean()` | cons_item [, period, weekAgo] |  |


### Consensus Median

Median of analyst estimates

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstMedian()` | cons_item [, period, weekAgo] |  |


### Consensus Standard Deviation

Standard Deviation of analysts estimates

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstStdDev()` | cons_item [, period, weekAgo] |  |


### Consensus Up

Number of analysts revising estimate up in past 75 days

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstUp()` | cons_item [, period, weekAgo] |  |


### Consensus Count

Number of analysts providing estimates for an item

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsEstCnt()` | cons_item [, period, weekAgo] |  |


## EPS Estimates

Earnings per share consensus estimates with statistics, number of analysts, and previous values for trend analysts.

### EPS Estimate Current Quarter

Number of analysts for current quarter EPS estimate. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsCurQ` |  |  |
| `CurQEPSMean` |  | Latest |
| `CurQEPS1WkAgo` |  | Week Ago |
| `CurQEPS4WkAgo` |  | 4 Weeks Ago |
| `CurQEPS8WkAgo` |  | 8 Weeks Ago |
| `CurQEPS13WkAgo` |  | 13 Weeks Ago |
| `CurQEPSHigh` |  | Latest |
| `CurQEPSLow` |  | Latest |
| `CurQEPSStdDev` |  | Latest |


### EPS Estimate Current Year

Number of analysts for current fiscal year EPS. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsCurFY` |  |  |
| `CurFYEPSMean` |  | Latest |
| `CurFYEPS1WkAgo` |  | Week Ago |
| `CurFYEPS4WkAgo` |  | 4 Weeks Ago |
| `CurFYEPS8WkAgo` |  | 8 Weeks Ago |
| `CurFYEPS13WkAgo` |  | 13 Weeks Ago |
| `CurFYEPSMedian` |  | Latest |
| `CurFYEPSHigh` |  | Latest |
| `CurFYEPSLow` |  | Latest |
| `CurFYEPSStdDev` |  | Latest |


### EPS Estimate Next Quarter

Number of analysts for next fiscal quarter EPS. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsNextQ` |  |  |
| `NextQEPSMean` |  | Latest |
| `NextQEPS1WkAgo` |  | Week Ago |
| `NextQEPS4WkAgo` |  | 4 Weeks Ago |
| `NextQEPS8WkAgo` |  | 8 Weeks Ago |
| `NextQEPS13WkAgo` |  | 13 Weeks Ago |
| `NextQEPSHigh` |  | Latest |
| `NextQEPSLow` |  | Latest |
| `NextQEPSStdDev` |  | Latest |


### EPS Estimate Next Year

Number of analysts for next fiscal year EPS. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsNextFY` |  |  |
| `NextFYEPSMean` |  | Latest |
| `NextFYEPS1WkAgo` |  | Week Ago |
| `NextFYEPS4WkAgo` |  | 4 Weeks Ago |
| `NextFYEPS8WkAgo` |  | 8 Weeks Ago |
| `NextFYEPS13WkAgo` |  | 13 Weeks Ago |
| `NextFYEPSMedian` |  | Latest |
| `NextFYEPSHigh` |  | Latest |
| `NextFYEPSLow` |  | Latest |
| `NextFYEPSStdDev` |  | Latest |


### EPS Estimate Other Years

EPS mean estimate 2 years

| Factor | Params | Variant |
|--------|--------|---------|
| `FY2EPSMean` |  | 2 Years |
| `FY3EPSMean` |  | 3 Years |


## Sales Estimates

Sales consensus estimates with statistics, number of analysts, and previous values for trend analysts.

### Sales Estimate Current Year

Number of analysts for current fiscal year sales. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsCurFYSales` |  |  |
| `CurFYSalesMean` |  | Latest |
| `CurFYSales1WkAgo` |  | Week Ago |
| `CurFYSales4WkAgo` |  | 4 Weeks Ago |
| `CurFYSales8WkAgo` |  | 8 Weeks Ago |
| `CurFYSales13WkAgo` |  | 13 Weeks Ago |
| `CurFYSalesMedian` |  | Latest |
| `CurFYSalesStdDev` |  | Latest |


### Sales Estimate Next Year

Number of analysts for next fiscal year sales. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsNextFYSales` |  |  |
| `NextFYSalesMean` |  | Latest |
| `NextFYSales1WkAgo` |  | Week Ago |
| `NextFYSales4WkAgo` |  | 4 Weeks Ago |
| `NextFYSales8WkAgo` |  | 8 Weeks Ago |
| `NextFYSales13WkAgo` |  | 13 Weeks Ago |
| `NextFYSalesMedian` |  | Latest |
| `NextFYSalesStdDev` |  | Latest |


### Sales Estimate Other Years

Sales estimate 2 years

| Factor | Params | Variant |
|--------|--------|---------|
| `FY2SalesMean` |  | 2 Years |
| `FY3SalesMean` |  | 3 Years |
| `NTMSalesMean` |  |  |


## Other Estimates

Other consensus mean estimates

### CapEx Estimate Mean

CapEx Estimate Mean Current Year

| Factor | Params | Variant |
|--------|--------|---------|
| `CapExEstCY` |  |  |
| `CapExEstNY` |  |  |
| `CapExEstY2` |  |  |
| `CapExEstY3` |  |  |


### EBITDA Estimate Mean

Average of analyst estimates for EBITDA for the Current Year

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAEstCY` |  | Current Year |
| `EBITDAEstNY` |  | Next Year |
| `EBITDAEstY2` |  | 2 Years |
| `EBITDAEstY3` |  | 3 Years |


### FCF Estimate Mean

Free cash flow estimate mean current year

| Factor | Params | Variant |
|--------|--------|---------|
| `FCFEstCY` |  | Current Year |
| `FCFEstNY` |  | Next Year |
| `FCFEstY2` |  | 2 years |
| `FCFEstY3` |  | 3 Years |


## EPS Revisions

Factors to indicate number of analysts revisions EPS consensus estimate Up or Down. NOTE: Data is only updated in the weekend

### EPS Revisions Current Quarter

Current Quarter Down Revisions, Last Week

| Factor | Params | Variant |
|--------|--------|---------|
| `CurQDnRevLastWk` |  | Past Week |
| `CurQUpRevLastWk` |  | Past Week |
| `CurQDnRev4WkAgo` |  | Past 4 Weeks |
| `CurQUpRev4WkAgo` |  | Past 4 Weeks |


### EPS Revisions Current Year

Current Fiscal Year Down Revisions, Last Week

| Factor | Params | Variant |
|--------|--------|---------|
| `CurFYDnRevLastWk` |  | Past Week |
| `CurFYUpRevLastWk` |  | Past Week |
| `CurFYDnRev4WkAgo` |  | Past 4 Weeks |
| `CurFYUpRev4WkAgo` |  | Past 4 Weeks |


### EPS Revisions Next Quarter

Next Quarter Down Revisions, Last Week

| Factor | Params | Variant |
|--------|--------|---------|
| `NextQDnRevLastWk` |  | Past Week |
| `NextQUpRevLastWk` |  | Past Week |
| `NextQDnRev4WkAgo` |  | Past 4 Weeks |
| `NextQUpRev4WkAgo` |  | Past 4 Weeks |


### EPS Revisions Next Year

Next Fiscal Year Down Revisions, Last Week

| Factor | Params | Variant |
|--------|--------|---------|
| `NextFYDnRevLastWk` |  | Past Week |
| `NextFYUpRevLastWk` |  | Past Week |
| `NextFYDnRev4WkAgo` |  | Past 4 Weeks |
| `NextFYUpRev4WkAgo` |  | Past 4 Weeks |


### Sum of EPS Revisions

Sum of  (No Analysts Up Revisions) - (No Analysts Dn revisions) in the past week.

| Factor | Params | Variant |
|--------|--------|---------|
| `TotRevisionsLastW` |  | Past Week |
| `TotRevisions4W` |  | Past 4 Weeks |


## Surprises

Analysts surprises

### Analyst EPS Surprise

EPS surprise (Est vs. Actual)

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSSurprise()` | offset, type |  |
| `Surprise%Q1` |  | Most Recent Quarter |
| `Surprise%Q2` |  | 2 Quarters Ago |
| `Surprise%Q3` |  | 3 Quarters Ago |
| `Surprise%Q4` |  | 4 Quarters Ago |
| `Surprise%Q5` |  | 5 Quarters Ago |
| `Surprise%Y1` |  | Most Recent Year |
| `Surprise%Y2` |  | 2 Years Ago |
| `Surprise%Y3` |  | 3 Years Ago |
| `Surprise%Y4` |  | 4 Years Ago |


### Analyst Sales Surprise

Sales Surprise in %

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesSurprise()` | offset, type |  |
| `SalesSurp%Q1` |  | Most Recent Quarter |
| `SalesSurp%Q2` |  | 2 Quarters Ago |
| `SalesSurp%Q3` |  | 3 Quarters Ago |
| `SalesSurp%Q4` |  | 4 Quarters Ago |
| `SalesSurp%Q5` |  | 5 Quarters Ago |
| `SalesSurp%Y1` |  | Most Recent Year |
| `SalesSurp%Y2` |  | 2 Years Ago |
| `SalesSurp%Y3` |  | 3 Years Ago |
| `SalesSurp%Y4` |  | 4 Years Ago |


### Unexpected Earnings (SUE)

Standardized Unexpected Earnings general formula

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSSUE()` | offset, type [, constraint] |  |
| `SUEQ1` |  | Most Recent Quarter |
| `SUEQ2` |  | 2 Quarter Ago |
| `SUEQ3` |  | 3 Quarters Ago |
| `SUEQ4` |  | 4 Quarter Ago |
| `SUEY1` |  | Most Recent Year |
| `SUEY2` |  | 2 Years Ago |
| `SUEY3` |  | 3 Years Ago |
| `SUEY4` |  | 4 Years Ago |


### Unexpected Sales (SUS)

Standardized Unexpected Sales general formula

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesSUS()` | offset, type [, constraint] |  |
| `SUSQ1` |  | Most Recent Quarter |
| `SUSQ2` |  | 2 Quarter Ago |
| `SUSQ3` |  | 3 Quarters Ago |
| `SUSQ4` |  | 4 Quarter Ago |
| `SUSY1` |  | Most Recent Year |
| `SUSY2` |  | 2 Years Ago |
| `SUSY3` |  | 3 Years Ago |
| `SUSY4` |  | 4 Years Ago |


## Historical

Analysts last estimates for previous periods and surprises compared to the Actuals

### Historical EPS Estimate

Historical mean EPS estimate.

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSEst()` | offset, type |  |
| `HistQ1EPSEst` |  | 1 Quarter Ago |
| `HistQ2EPSEst` |  | 2 Quarters Ago |
| `HistQ3EPSEst` |  | 3 Quarters Ago |
| `HistQ4EPSEst` |  | 4 Quarters Ago |
| `HistQ5EPSEst` |  | 5 Quarters Ago |


### Historical Estimate Number of Analysts

Historical EPS Estimate Number of Analysts

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSHistEstCnt()` | offset, type |  |
| `SalesHistEstCnt()` | offset, type |  |


### Historical Estimate Standard Deviation

Historical EPS Estimate Standard Deviation

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSHistEstSD()` | offset, type |  |
| `SalesHistEstSD()` | offset, type |  |


### Historical Sales Estimate

Historical Sales Estimate

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesEst()` | offset, type |  |
| `SalesEstQ1` |  | 1 Quarter Ago |
| `SalesEstQ2` |  | 2 Quarters Ago |
| `SalesEstQ3` |  | 3 Quarters Ago |
| `SalesEstQ4` |  | 4 Quarters Ago |
| `SalesEstQ5` |  | 5 Quarters Ago |


### Historical EPS Difference

Historical Quarter Difference (Actual - Estimate), 1 Quarter Ago

| Factor | Params | Variant |
|--------|--------|---------|
| `HistQ1Difference` |  | 1 Quarter Ago |
| `HistQ2Difference` |  | 2 Quarters Ago |
| `HistQ3Difference` |  | 3 Quarters Ago |
| `HistQ4Difference` |  | 4 Quarters Ago |
| `HistQ5Difference` |  | 5 Quarters Ago |


## Recs & Opinions

Analysts average recommendation and long-term growth estimate.

### Long Term EPS Growth

This is the number of analysts who are reporting a long term earnings per share growth rate. If a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsLTGrthRt` |  |  |
| `LTGrthMean` |  | Latest |
| `LTGrth1WkAgo` |  | Week Ago |
| `LTGrth4WkAgo` |  | 4 Weeks Ago |
| `LTGrth8WkAgo` |  | 8 Weeks Ago |
| `LTGrth13WkAgo` |  | 13 Weeks Ago |
| `LTGrthHigh` |  | Latest |
| `LTGrthLow` |  | Latest |
| `LTGrthStdDev` |  | Latest |


### Price Target

Number of analysts giving price target estimates. Note: if a security has no analysts, this factor returns NA, not 0.

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnalystsPriceTarget` |  |  |
| `PriceTarget4WkAgo` |  |  |
| `PriceTargetHi` |  |  |
| `PriceTargetLo` |  |  |
| `PriceTargetMean` |  |  |
| `PriceTargetStdDev` |  |  |


### Average Recommendation

Average Recommendation on a 1-3 linear scale, where 1 is a strong buy, 3 a sell. For CapitalIQ the range is 1-5.

| Factor | Params | Variant |
|--------|--------|---------|
| `AvgRec` |  | Current |
| `AvgRec1WkAgo` |  | 1 Week Ago |
| `AvgRec4WkAgo` |  | 4 Weeks Ago |
| `AvgRec8WkAgo` |  | 8 Weeks Ago |
| `AvgRec13WkAgo` |  | 13 Weeks Ago |


### Recommendation Function

Consensus recommendation

| Factor | Params | Variant |
|--------|--------|---------|
| `ConsRec()` | rec_stat [, weekAgo] |  |

