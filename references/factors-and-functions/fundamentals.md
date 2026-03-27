# Fundamentals

Other company fundamental data that is not a direct financial statement line item from filings or press releases.

## Actuals

Actuals are companies' historical financial data, such as earnings, sales, and net income. Unlike fundamentals that come from official filings submitted to government agencies, Actuals are collected primarily from company press releases or from brokers.

### Actual Functions

Retrieve the actual item for a specific period indicated by the offset and period type

| Factor | Params | Variant |
|--------|--------|---------|
| `Actual()` | actual_item, offset, type |  |
| `ActualQ()` | actual_item | Latest Quarter |
| `ActualPQ()` | actual_item | Previous Quarter |
| `ActualPYQ()` | actual_item | Previous Quarter 1 Year Ago |
| `ActualTTM()` | actual_item | Trailing 12 Months |
| `ActualPTM()` | actual_item | Previous Trailing 12 Months |
| `ActualA()` | actual_item | Latest Year |
| `ActualPY()` | actual_item | Previous Year |
| `ActualGr%PQ()` | actual_item | Growth Q |
| `ActualGr%PYQ()` | actual_item | Growth PYQ |
| `ActualGr%TTM()` | actual_item | Growth TTM |
| `ActualGr%A()` | actual_item | Growth Annual |


### Sales Actual

Historical (Actual) Sales

| Factor | Params | Variant |
|--------|--------|---------|
| `SalesActual()` | offset, type |  |
| `SalesActualTTM` |  | Trailing 12 Months |
| `SalesActualPTM` |  | Previous Trailing 12 Months |
| `SalesActualGr%TTM` |  | Growth TTM |
| `SalesActualGr%PYQ` |  | Growth PYQ |
| `SalesActualQ1` |  | 1 Quarter Ago |
| `SalesActualQ2` |  | 2 Quarters Ago |
| `SalesActualQ3` |  | 3 Quarters Ago |
| `SalesActualQ4` |  | 4 Quarters Ago |
| `SalesActualQ5` |  | 5 Quarters Ago |


### EPS Actual

Historical (Actual) EPS

| Factor | Params | Variant |
|--------|--------|---------|
| `EPSActual()` | offset, type |  |
| `EPSActualTTM` |  | Trailing 12 Months |
| `EPSActualPTM` |  | Previous Trailing 12 Months |
| `EPSActualGr%TTM` |  | Growth TTM |
| `EPSActualGr%PYQ` |  | Growth PYQ |
| `HistQ1EPSActual` |  | 1 Quarter Ago |
| `HistQ2EPSActual` |  | 2 Quarters Ago |
| `HistQ3EPSActual` |  | 3 Quarters Ago |
| `HistQ4EPSActual` |  | 4 Quarters Ago |
| `HistQ5EPSActual` |  | 5 Quarters Ago |


### EBITDA Actual

EBITDA Actual function

| Factor | Params | Variant |
|--------|--------|---------|
| `EBITDAActual()` | offset, type |  |
| `EBITDAActualTTM` |  | Trailing 12 Months |
| `EBITDAActualPTM` |  | Previous Trailing 12 Months |
| `EBITDAActualGr%TTM` |  | Growth TTM |
| `EBITDAActualGr%PYQ` |  | Growth PYQ |


### Actual Latest

Calendar days since analysts actuals for the most recent quarter were available from the data vendor.

NOTE: analysts actuals can precede SEC filings

| Factor | Params | Variant |
|--------|--------|---------|
| `LatestActualDays` |  | Latest Quarter |
| `LatestActualPeriodDate` |  | Latest Quarter |


## Company

Qualitative and informational data about the company. Includes country of domicile and number of employees.

### Country Code

Country of domicile

| Factor | Params | Variant |
|--------|--------|---------|
| `CountryCode` |  |  |


### Country of domicile

Returns 1(TRUE) if the country of domicile matches any of the countries whose codes are specified,  0 (FALSE) otherwise. Use commas or spaces to separate your list of up to 20 codes. See Full Description for a list country codes.

| Factor | Params | Variant |
|--------|--------|---------|
| `Country()` | "cid, cid, cid, ..." |  |


### Exchange Country

Returns 1 (TRUE) if the country of the exchange where the security trades matches any of the countries whose codes are specified, 0 (FALSE) otherwise. Use commas or spaces to separate your list of up to 20 codes. See Full Description for a list of country codes.

| Factor | Params | Variant |
|--------|--------|---------|
| `ExchCountry()` | "cid, cid, cid, ..." |  |


### Number of employees

Number of employees.

| Factor | Params | Variant |
|--------|--------|---------|
| `NoEmp()` | offset, type[, NAHandling] |  |
| `NoEmpA` |  | Latest Year |
| `NoEmpPY` |  | Previous Year |
| `NoEmpGr%A` |  | Growth Annual |
| `NoEmpGr%3Y` |  | Three Year Annualized Growth |
| `NoEmpGr%5Y` |  | Five Year Annualized Growth |
| `NoEmpGr%10Y` |  | Ten Year Annualized Growth |
| `NoEmp3YAvg` |  | Three Year Average |
| `NoEmp5YAvg` |  | Five Year Average |


### Number of Periods

Number of Historical Periods, Annual

| Factor | Params | Variant |
|--------|--------|---------|
| `#APeriods` |  | Annual Periods |
| `#QPeriods` |  | Interim Periods |


### Earnings Release

Returns 0 or the number of days the filing is late (over 40 days for Q and over 75 for K). If the company has no filing data NA is returned. NOTE: This is an estimate. See the Full Description for more details

| Factor | Params | Variant |
|--------|--------|---------|
| `DaysLate` |  | Next Quarter |
| `WeeksToQ` |  | Weeks To Quarter |
| `WeeksToY` |  | Weeks To Year |
| `WeeksIntoQ` |  | Weeks Into Quarter |


## Corporate Actions

Flags and data relating to the timing and history of corporate events, including splits and M&A.

### Corporate Actions (ICE Data)

Returns the days since a M&A (incl spinoff) corporate action has been announced or NA. Equivalent to PendingCorpAct(#MANDA, #ANNCEDAYS)

| Factor | Params | Variant |
|--------|--------|---------|
| `DaysFromMergerAnn` |  |  |
| `PastCorpAct()` | ca_type [, ca_status, lookback, ca_retvalue] |  |
| `PendingCorpAct()` | ca_type [, ca_retvalue] |  |


### Dividends Days

Days since the last dividend ex-date. Always a positive number or NA

| Factor | Params | Variant |
|--------|--------|---------|
| `DaysFromDivEx` |  |  |
| `DaysFromDivPay` |  |  |
| `DaysToDivEx` |  |  |
| `DaysToDivPay` |  |  |


### Future Dividend and Split Factor

Returns the product of all the splits and dividends in the future of the observation date (As-Of Date)

| Factor | Params | Variant |
|--------|--------|---------|
| `FutureDivSplitFactor` |  |  |


### Future Dividend Factor

Returns the product of all the dividends in the future of the observation date (As-Of Date)

| Factor | Params | Variant |
|--------|--------|---------|
| `FutureDivFactor` |  |  |


### Future Split Factor

Returns the product of all the splits in the future of the observation date (As-Of Date)

| Factor | Params | Variant |
|--------|--------|---------|
| `FutureSplitFactor` |  |  |


### Splits

Returns the number of splits in the past or future number of days

| Factor | Params | Variant |
|--------|--------|---------|
| `SplitCount()` | days |  |
| `SplitFactor()` | days |  |
| `Splits()` | days [, countFlag] |  |


## Dividends

Dividend-related data, including yield and IAD.

### Dividend Growth

Dividend Percent Change, Year Over Year (%)

| Factor | Params | Variant |
|--------|--------|---------|
| `Div%ChgA` |  | Latest Year |
| `Div%ChgPYQ` |  | Latest Quarter vs 1 Year Ago |
| `Div%ChgTTM` |  | Trailing Twelve Months |
| `Div3YCGr%` |  | 3 Years |
| `Div5YCGr%` |  | 5 Years |


### Dividends in a Filing Period

Returns the sum (or count) of the dividends per share that were paid in the period specified. By default it returns the sum of REGULAR dividends using EX DATES. See Full description for details.

| Factor | Params | Variant |
|--------|--------|---------|
| `DivPS()` | offset, type [, div_type , div_dt, cnt_flag] |  |
| `DivPS5YAvg` |  | 5 Years |
| `DivPSNextQ` |  | Next Quarter |
| `DivPSNextQCnt` |  | Next Quarter |
| `DivPSQ` |  | Latest Quarter |
| `DivPSTTM` |  | Trailing 12 Months |


### Dividends in a Time Period

Returns the sum of all regular dividends with ex-dates in the past calendar year.  It's equivalent to DivPSDays(365,0,#Regular,#ExDate)

| Factor | Params | Variant |
|--------|--------|---------|
| `DivPS52W` |  | 52 Weeks |
| `DivPSDays()` | days [, offset, div_type, div_dt, cnt_flag] |  |


### Indicated Annual Dividend

Indicated Annual Dividend. This is a forward looking number used to calculate yield. It can also be used to find companies increasing their dividends.

| Factor | Params | Variant |
|--------|--------|---------|
| `IAD` |  | Next Year |
| `IAD13W` |  | 13 Weeks Ago |
| `IAD26W` |  | 26 Weeks Ago |
| `IAD52W` |  | 52 Weeks Ago |


## Filings Related

Information about the earnings reports filed by the company to regulatory agencies.

### Actual Interim Days

Days in the filing period for the given interim offset. Usually 91 or 92 for quarterly, 182 or 183 for semiannual.

| Factor | Params | Variant |
|--------|--------|---------|
| `ActualInterimDays()` | offset | Quarter |


### Interim Months

Months in the filing period for the given interim offset (the offset parameter is the number of interim periods you want to look back). Always returns either 3 or 6: 3 for stocks that report quarterly, 6 for those that report semiannually. This function will always return 3 for Compustat interims.

| Factor | Params | Variant |
|--------|--------|---------|
| `InterimMonths()` | offset | Quarter |


### Percent of NAs in Period

Returns the percent of line items pulled that are missing. TTM returns an average of the periods.

| Factor | Params | Variant |
|--------|--------|---------|
| `PerNAPct()` | offset, type |  |
| `PerNAPctQ` |  | Latest Quarter |
| `PerNAPctPQ` |  | Previous Quarter |
| `PerNAPctPYQ` |  | Previous Quarter 1 Year Ago |
| `PerNAPctTTM` |  | Trailing 12 Months |
| `PerNAPctPTM` |  | Previous Trailing 12 Months |
| `PerNAPctA` |  | Latest Year |
| `PerNAPctPY` |  | Previous Year |


### Complete Flag

Complete Statement. Set to TRUE (1) if the latest filing is final and, typically, filed with SEC. FALSE (0) if it contains pre-announcement data. When CompleteStmt is FALSE our''fallback'' mechanism kicks in for most ratios that evaluate to N/A because of incomplete data.

| Factor | Params | Variant |
|--------|--------|---------|
| `CompleteStmt` |  | Latest Quarter |


### Stale Flag

Returns 1 (TRUE) when there's no data in the database for the latest period that is publicly available from a press release or SEC filing

| Factor | Params | Variant |
|--------|--------|---------|
| `StaleStmt` |  | Latest Quarter |


### Latest in Database

Returns the number of days it took the company to announce the Prev Year Q filing (announce date - period end)

| Factor | Params | Variant |
|--------|--------|---------|
| `AnnounceDaysPYQ` |  | Previous Year Q |
| `AnnounceDaysQ` |  | Latest Quarter |
| `PeriodDateA` |  | Latest Year |
| `PeriodDateQ` |  | Latest Quarter |
| `QtrComplete` |  | Latest Quarter |


### Latest (Any Source)

The date the latest period was first filed by the company with the SEC. This date may be before any data appears for the as-of date of your analysis due to vendor delays in processing the filing.

| Factor | Params | Variant |
|--------|--------|---------|
| `LatestFilingDate` |  | Latest Quarter |
| `LatestNewsDate` |  | Latest Quarter |
| `LatestPeriodDate` |  | Latest Quarter |


## Listing Related

Factors and functions related with the traded listing or stock

### Exchange Code

Returns the point in time exchange code where the listing trades

| Factor | Params | Variant |
|--------|--------|---------|
| `ExchangeCode` |  |  |


### FIGI

Returns 1(TRUE) if the FIGI is in the list, 0 (FALSE) otherwise. This searches the global share class level FIGIs. To add FIGIs to the screen report visit Screen Reports.

| Factor | Params | Variant |
|--------|--------|---------|
| `FIGI()` | "figi1, figi2..." |  |


### FIGI Identifier

Returns the Country Composite level FIGI identifier.

| Factor | Params | Variant |
|--------|--------|---------|
| `ccFIGI` |  |  |
| `scFIGI` |  |  |


### Is ADR

Returns 1 (TRUE) if the stock is an American Depository Receipt (ADR)

| Factor | Params | Variant |
|--------|--------|---------|
| `IsADR` |  |  |


### Is MLP

Returns 1 (TRUE) if the stock is a Master Limited Partnership (MLP) in USA or Canada.

| Factor | Params | Variant |
|--------|--------|---------|
| `IsMLP` |  |  |


### Is Over The Counter (OTC)

Returns 1 (TRUE) if the stock trades OTC in the USA.

| Factor | Params | Variant |
|--------|--------|---------|
| `IsOTC` |  |  |


### Is Primary

Returns 1 (TRUE) if the stock is the primary listing for the company, i.e. not a foreign stock.

| Factor | Params | Variant |
|--------|--------|---------|
| `IsPrimary` |  |  |


### Security Type

Returns the code of the security. For example: Common, Unit, MLP, BDC, etc. See Full Description for the codes

| Factor | Params | Variant |
|--------|--------|---------|
| `SecurityType` |  |  |


### Ticker

Returns 1(TRUE) if the ticker is in the list, 0 (FALSE) otherwise. Use commas or spaces to separate your list. You can also use wildcards * to match any string or ? for any character

| Factor | Params | Variant |
|--------|--------|---------|
| `Ticker()` | "ticker1, ticker2, ..." |  |


### Unique Stock Identifier

Returns the internal ID of the current stock or ETF. Can be used to create any number samples in conjunction with modulus function Mod()

| Factor | Params | Variant |
|--------|--------|---------|
| `StockID` |  |  |


## Insider & Institutional

Data relating to institutional & insider ownership of a company's shares.

### Insider Factors

Insider total shares purchased past 6 months (positive number in millions)

| Factor | Params | Variant |
|--------|--------|---------|
| `Ins#ShrPurch` |  |  |
| `Ins#ShrSold` |  |  |
| `InsBuyTrans` |  |  |
| `Insider#Own` |  |  |
| `Insider%Own` |  |  |
| `InsNetShrPurch` |  |  |
| `InsNetTrans` |  |  |
| `InsSelTrans` |  |  |


### Insider Functions

Shares bought by insiders past 12 months (in millions)

| Factor | Params | Variant |
|--------|--------|---------|
| `InsiderBuySh12M()` | mo_offset |  |
| `InsiderBuySh1M()` | mo_offset |  |
| `InsiderBuySh3M()` | mo_offset |  |
| `InsiderBuySh6M()` | mo_offset |  |
| `InsiderBuyTran12M()` | mo_offset |  |
| `InsiderBuyTran1M()` | mo_offset |  |
| `InsiderBuyTran3M()` | mo_offset |  |
| `InsiderBuyTran6M()` | mo_offset |  |
| `InsiderSellSh12M()` | mo_offset |  |
| `InsiderSellSh1M()` | mo_offset |  |
| `InsiderSellSh3M()` | mo_offset |  |
| `InsiderSellSh6M()` | mo_offset |  |
| `InsiderSellTran12M()` | mo_offset |  |
| `InsiderSellTran1M()` | mo_offset |  |
| `InsiderSellTran3M()` | mo_offset |  |
| `InsiderSellTran6M()` | mo_offset |  |
| `InsiderUniqBuy1M()` | mo_offset |  |
| `InsiderUniqBuy3M()` | mo_offset |  |
| `InsiderUniqSell1M()` | mo_offset |  |
| `InsiderUniqSell3M()` | mo_offset |  |


### Institutional Factors

The total number of investors who own shares of the company

| Factor | Params | Variant |
|--------|--------|---------|
| `#Institution` |  | Most Recent |
| `Inst#ShsOwn` |  |  |
| `Inst#ShsOwnPQ` |  | Previous Quarter |
| `Inst#ShsPurch` |  |  |
| `Inst#ShsPurchPQ` |  | Previous Quarter |
| `Inst#ShsSold` |  |  |
| `Inst#ShsSoldPQ` |  | Previous Quarter |
| `Inst%Own` |  |  |
| `Inst%OwnPQ` |  | Previous Quarter |
| `InstNetPurch` |  |  |
| `InstNetPurchPQ` |  | Previous Quarter |


### Institutional Functions

The number of investors who purchased shares of the company during the period

| Factor | Params | Variant |
|--------|--------|---------|
| `InstitutionalBuyers()` | period_offset |  |
| `InstitutionalClosed()` | period_offset |  |
| `InstitutionalHolders()` | period_offset |  |
| `InstitutionalNewBuyers()` | period_offset |  |
| `InstitutionalPctChg()` | period_offset |  |
| `InstitutionalPctOwn()` | period_offset |  |
| `InstitutionalSellers()` | period_offset |  |
| `InstitutionalShsBought()` | period_offset |  |
| `InstitutionalShsHeld()` | period_offset |  |
| `InstitutionalShsNet()` | period_offset |  |
| `InstitutionalShsSold()` | period_offset |  |


## Short Interest

Data relating to the short interest of a company's shares.

### Short Interest

Short Interest, Current Month Position (millions)

USA only

| Factor | Params | Variant |
|--------|--------|---------|
| `SICM` |  | Latest |
| `SIPM` |  | 1 Month Ago |
| `SIPM2` |  | 2 Months Ago |
| `SIPM3` |  | 3 Months Ago |


### Short Interest Percent of Float

Short Interest, Percent of Float (%)

USA only

| Factor | Params | Variant |
|--------|--------|---------|
| `SI%Float` |  | Latest |
| `SI%FloatPM` |  | 1 Month Ago |
| `SI%FloatPM2` |  | 2 Months Ago |
| `SI%FloatPM3` |  | 3 Months Ago |


### Short Interest Percent of Shares Outstanding

Short Interest, Percent of Shares Outstanding (%)

USA only

| Factor | Params | Variant |
|--------|--------|---------|
| `SI%ShsOut` |  | Latest |
| `SI%ShsOutPM` |  | 1 Month Ago |
| `SI%ShsOutPM2` |  | 2 Months Ago |
| `SI%ShsOutPM3` |  | 3 Months Ago |


### Short Interest Ratio

Short Interest Ratio

USA only

| Factor | Params | Variant |
|--------|--------|---------|
| `SIRatio` |  | Latest |
| `SIRatioPM` |  | 1 Month Ago |
| `SIRatioPM2` |  | 2 Months Ago |
| `SIRatioPM3` |  | 3 Months Ago |


### Short Interest, Percent Change

Short Interest, One Month Percent Change (%)

USA only

| Factor | Params | Variant |
|--------|--------|---------|
| `SI1Mo%Chg` |  |  |

