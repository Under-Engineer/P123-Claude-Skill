# Advanced Functions

Advanced functions that provide things like summary statistics, ranks, and other specific analytics.

## AI Factor

Functions that return AI model predictions

### Predictions

Returns the inferences (predictions) of your trained Predictor. Mainly for use to rebalance but it can also be used in backtests with some restrictions.

| Factor | Params | Variant |
|--------|--------|---------|
| `AIFactor()` | "AI Factor Name", "Predictor Name" |  |


### Validation Predictions

Returns the saved inference (prediction) of your model's validation

| Factor | Params | Variant |
|--------|--------|---------|
| `AIFactorValidation()` | "AI Factor Name", "Model Name"[, "dup_id"] |  |


## Ranking

Functions that return the rank from a ranking system.

### Other Rank

Returns the rank position for the named Ranking System. You can specify one of your systems or one of our pre-built ranking systems. Example:

RatingPos("Momentum Value")<10

NOTE: A maximum of 3 Rating/RatingPos functions can be used for a request.

| Factor | Params | Variant |
|--------|--------|---------|
| `RatingPos()` | "RankName" |  |
| `Rating()` | "RankName" |  |


### Previous Rank

Historical weekly rank position based on the selected ranking system. Weekly ranks are updated every Saturday.

weeksAgo: number of weeks from 0-261.

| Factor | Params | Variant |
|--------|--------|---------|
| `RankPosPrev()` | weeksAgo |  |
| `RankPrev()` | weeksAgo |  |


### Latest Rank

Latest stock rank updated daily Tuesday-Saturday. Usage examples:

Portfolios and Sims: to sell a position when rank drops below 60, enter the following SELL rule:

Rank < 60

Screener: to screen for stocks with a Rank above 90 select the Ranking System to use and enter the following rule:

Rank > 90

| Factor | Params | Variant |
|--------|--------|---------|
| `Rank` |  |  |
| `RankPos` |  |  |
| `GetRank()` | "ticker" |  |
| `GetRankPos()` | "ticker" |  |


### Rank Bars

Returns the number of bars of the last rank data. NOTE: A "bar" is a trading day. Therefore there are 5 bars in a week with no holidays.

| Factor | Params | Variant |
|--------|--------|---------|
| `RankBars` |  |  |


### Node Rank

Returns the node rank within a ranking system. Please see the Full Description for details and examples.

| Factor | Params | Variant |
|--------|--------|---------|
| `NodeRank()` | "name" |  |


## FHist Functions

Functions that calculate Point In Time values (PIT) by changing the observation date. An example use case for these functions is to find stocks that are cheap relative to their previous valuations.

### Historical Average

Returns the average of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistAvg()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Max

Returns the maximum value of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistMax()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Median

Returns the median of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistMed()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Min

Returns the minimum value of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistMin()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Relative Standard Deviation

Returns the RSD of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistRelStdDev()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Standard Deviation

Returns the SD of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistStdDev()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Historical Sum

Returns the sum of 'formula' sampled multiple times in the past. Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistSum()` | "formula", samples [, weeks_increment=1, NA_pct=20] |  |


### Point In Time Value

Returns the value of 'formula' calculated in the past (or future when using negative values). Split/dividend sensitive values adjusted to the as-of date (observation date).

| Factor | Params | Variant |
|--------|--------|---------|
| `FHist()` | "formula", weeksAgo |  |


## Loop Functions

Functions that operate on historical values using a loop formula which must contain the CTR iterator. Example use cases for these functions include counting how many quarters have positive cashflow, and finding companies that have increased their dividend every year.

### Loop Average

Evaluates the "formula" parameter a number of times and return the average. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopAvg()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Max

Evaluates the "formula" parameter a number of times and return the maximum value. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopMax()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Median

Evaluates the "formula" parameter a number of times and returns the median value. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopMedian()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Min

Evaluates the "formula" parameter a number of times and returns the minimum value. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopMin()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Product

Evaluates the "formula" parameter a number of times and returns the product of the values. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopProd()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Rel Standard Deviation

Evaluates the "formula" parameter a number of times and returns the relative standard deviation. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopRelStdDev()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Standard Deviation

Evaluates the "formula" parameter a number of times and returns the standard deviation. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopStdDev()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


### Loop Streak

Evaluates the "formula" parameter a number of times and returns the streak count.  By default it returns the most recent streak of positive values. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopStreak()` | "formula(CTR)", iterations[, start=0, increment=1, streak=#Positive, recent=TRUE] |  |


### Loop Sum

Evaluates the "formula" parameter a number of times and returns the sum of the values. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopSum()` | "formula(CTR)", iterations[, start=0, increment=1, noNAs=FALSE, break=FALSE] |  |


## Loop Regression

Functions that calculate regressions on historical values using a loop formula which must contain the CTR iterator. Use cases for these functions include finding stocks with upward, well defined trends for sales.

### Linear Regression using Loop

Executes the "formula" parameter a number of times and operates a regression on the set of values. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LinReg()` | "Formula(CTR)", iterations[, start, increment] |  |


### Linear XY Regression using Loop

Executes the "formula" parameter a number of times and operates a bivariate regression on the set of values. A special CTR variable must be used inside "formula".

| Factor | Params | Variant |
|--------|--------|---------|
| `LinRegXY()` | "X-Formula(CTR)", "Y-Formula(CTR)", iterations[, start, increment] |  |


## Relative vs. History

Functions that compare and normalize values longitudinally against historical values for the same stock.

### FHist Rank

Returns the percentile rank from 0 to 100 of most recent value vs. previous PIT values.

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistRank()` | "formula", samples[, weeks_increment=1, sort=#DESC, sort_style=#Top, NA_value=NA, NA_pct=20] |  |


### FHist Relative

Returns the relative value from 0 to 1 of most recent value vs. previous minimum and maximum PIT values.

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistRel()` | "formula", samples [, weeks_increment=1, NA_value=NA, NA_Pct=20] |  |


### FHist ZScore

Returns the zscore of most recent value vs. previous PIT values.

| Factor | Params | Variant |
|--------|--------|---------|
| `FHistZScore()` | "formula", samples, weeks_increment=1, clip=3.5, NA_value=NA, NA_pct=20 |  |


### Loop Rank

Returns the rank of most recent value of the Loop formula vs. previous values calculated by iterating the CTR variable.

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopRank()` | “formula(CTR)”, iterations[, start=0, incr=1, sort=#DESC, sort_style=#Top, NA_value=NA, NA_Pct=20] |  |


### Loop Relative

Returns the relative value from 0 to 1 of most recent value of the Loop formula vs. previous minimum and maximum values calculated by iterating the CTR variable.

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopRel()` | "formula(CTR)", iterations[, start=0, increment=0, NA_value=NA, NA_pct=20] |  |


### Loop ZScore

Returns the zscore of most recent value of the Loop formula vs. previous values calculated by iterating the CTR variable.

| Factor | Params | Variant |
|--------|--------|---------|
| `LoopZScore()` | "formula(CTR)", iterations[, start=0, increment=1, clip=3.5, NA_value=NA, NA_pct=20] |  |


## Relative vs. Group

Functions that compare and normalize values cross-sectionally vs. other stocks in a group. Use cases for these functions include screening for stocks that are in the top 10% for a metric in their sector.

### Order in a Group

Sorts stocks based on formula and returns the position in the array.

| Factor | Params | Variant |
|--------|--------|---------|
| `FOrder()` | "formula" [, scope=#All, sort=#DESC, distinct=FALSE, incl_na=#InclNA] |  |


### Rank in a Group

Ranks stocks based on a formula and returns the percentile.

| Factor | Params | Variant |
|--------|--------|---------|
| `FRank()` | "formula"[, scope=#All, sort=#DESC, incl_na=#InclNA, sort_style=#Top] |  |


### ZScore in a Group

Calculates how many standard deviations the value from the formula is from the mean

| Factor | Params | Variant |
|--------|--------|---------|
| `ZScore()` | "formula"[, scope=#All, outlier_pct=7.5, na_value=0, max_zscore=3.5] |  |


## Group Summary Statistics

Functions that calculate cross-sectional summary statistics for a group. An example use case for these functions is to find companies that are cheap relative to their industry or sub-sector.

### Group Average

Returns the average or cap-weighted average for each scope

| Factor | Params | Variant |
|--------|--------|---------|
| `Aggregate()` | "formula", scope [, method, outlier_pct, outlier_handl, excl_zero, excl_adrs, median_fallback] |  |


### Group Count

Counts the number of stocks in each scope where formula is true (non 0)

| Factor | Params | Variant |
|--------|--------|---------|
| `FCount()` | "formula" [, scope] |  |


### Group Median

Returns the median value of the formula in each scope

| Factor | Params | Variant |
|--------|--------|---------|
| `FMedian()` | "formula" [, scope, excl_zero] |  |


### Group Sum

Returns the sum value of the formula in each scope

| Factor | Params | Variant |
|--------|--------|---------|
| `FSum()` | "formula" [, scope] |  |


## Screener Only

Misc functions that only work in the screener.

### Screen Holdings

Runs the screen specified in the first parameter. If top>0 then only the specified top stocks are returned. With this you can create screen-of-screens.

Screen("Graham",7) Or Screen("Lynch",7)

| Factor | Params | Variant |
|--------|--------|---------|
| `Screen()` | "ScreenName", top |  |


### Sector Count

Running count of stocks in the sector. This rule must be the last rule in the screen.

| Factor | Params | Variant |
|--------|--------|---------|
| `SecCount` |  |  |
| `SubSecCount` |  |  |


### Industry Count

Running count of stocks in the industry. This rule must be the last rule in the screen.

| Factor | Params | Variant |
|--------|--------|---------|
| `IndCount` |  |  |
| `SubIndCount` |  |  |


### Show Correlation Matrix in report

This function produces a correlation matrix in the screen report

| Factor | Params | Variant |
|--------|--------|---------|
| `ShowCorrel()` | period , samples |  |


### Show/Set Variable function

Sets the variable @myvar to expression, returns TRUE, and displays @myvar in the screen report.

| Factor | Params | Variant |
|--------|--------|---------|
| `ShowVar()` | @myvar, expression |  |


## Watchlists, Holdings, & Opinions

Functions that access holdings in watchlists, portfolios, or accounts as well as functions that access stock opinions.

### Recent Opinion

Returns your most recent opinion for the stock or NA

| Factor | Params | Variant |
|--------|--------|---------|
| `Opinion` |  |  |
| `Opinion%Chg` |  |  |
| `OpinionBars` |  |  |
| `OpinionDays` |  |  |


### Watchlist Holdings

Returns TRUE if the stock is currently in your watchlist.

| Factor | Params | Variant |
|--------|--------|---------|
| `WatchlistCurrent()` | "Name" |  |
| `Watchlist()` | id1[, .., id10] |  |
| `WatchlistClose()` | id1[, .., id10] |  |
| `WatchlistCloseBar()` | id1[, .., id10] |  |
| `WatchlistOpen()` | id1[, .., id10] |  |
| `WatchlistOpenBar()` | id1[, .., id10] |  |


### Account Holdings

Return TRUE if stock being analyzed is an open position. For the id parameters use either the name in quotes, or the numerical id.

| Factor | Params | Variant |
|--------|--------|---------|
| `Account()` | id1[, .., id10] |  |
| `AccountClose()` | id1[, .., id10] |  |
| `AccountCloseBar()` | id1[, .., id10] |  |
| `AccountOpen()` | id1[, .., id10] |  |
| `AccountOpenBar()` | id1[, .., id10] |  |


### Portfolio Holdings

Return TRUE if stock being analyzed is an open position. For the id parameters use either the name in quotes, or the numerical id.

| Factor | Params | Variant |
|--------|--------|---------|
| `Portfolio()` | id1[, .., id10] |  |
| `PortfolioClose()` | id1[, .., id10] |  |
| `PortfolioCloseBar()` | id1[, .., id10] |  |
| `PortfolioOpen()` | id1[, .., id10] |  |
| `PortfolioOpenBar()` | id1[, .., id10] |  |

