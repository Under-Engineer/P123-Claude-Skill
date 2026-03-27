# Technical

Functions to calculate and create information and triggers based on price or volume.

## Performance

Price changes and total return.

### Currency Adjustment Ratio

Ratio to normalize a stock performance to the currency of your system

| Factor | Params | Variant |
|--------|--------|---------|
| `FXPerf()` | bars [, offset] |  |


### Future Return

Future total return

| Factor | Params | Variant |
|--------|--------|---------|
| `Future%Chg()` | bars [, series] | Series Dependent |
| `Future%Chg_D()` | days [, series] | Weekday |
| `FutureRel%Chg()` | bars [, series] | Series Dependent |
| `FutureRel%Chg_D()` | days [, series] | Weekday |


### Percent From Average

Percent from SMA (incl div)

| Factor | Params | Variant |
|--------|--------|---------|
| `SMAPct()` | bars [, series] | Series Dependent |
| `SMAPct_W()` | weeks [, series] | Weekly |


### Percent From Hi/Lo

Percent from high in the period (incl div)

| Factor | Params | Variant |
|--------|--------|---------|
| `HighPct()` | bars [, series] | Series Dependent |
| `HighPct_W()` | weeks [, series] | Weekly |
| `LowPct()` | bars [, series] | Series Dependent |
| `LowPct_W()` | weeks [, series] | Weekly |
| `Pct3MH` |  | 3 Months |
| `Pct3ML` |  | 3 Months |
| `Pct4WH` |  | 4 Weeks |
| `Pct4WL` |  | 4 Weeks |
| `Pct52WH` |  | 52 Weeks |
| `Pct52WL` |  | 52 Weeks |


### Return Incl Div (Relative)

Total return relative to the benchmark or other series

| Factor | Params | Variant |
|--------|--------|---------|
| `Rel%Chg()` | bars [, series] | Series Dependent |
| `Rel%Chg_D()` | bars [, series] | Weekday |


### Return Incl Div (Total Return)

Total return (includes dividends) in the period specified

| Factor | Params | Variant |
|--------|--------|---------|
| `Ret%Chg()` | bars [, offset, series] | Series Dependent |
| `Ret%Chg_D()` | bars [, offset, series] | Weekday |
| `Ret1W%Chg` |  | 1 Week |
| `Ret1Y%Chg` |  | 1 Year |
| `Ret2Y%Chg` |  | 2 Years |
| `Ret3M%Chg` |  | 3 Months |
| `Ret4W%Chg` |  | 4 Weeks |
| `Ret6M%Chg` |  | 6 Months |


### Return Excl Div

Price percent change during the period. Dividends are not included (see Ret%Chg if you want dividends included)

| Factor | Params | Variant |
|--------|--------|---------|
| `Pr4W%Chg` |  | 4 Weeks |
| `Pr4WRel%Chg` |  | 4 Weeks |
| `Pr13W%Chg` |  | 13 Weeks |
| `Pr13WRel%Chg` |  | 13 Weeks |
| `Pr26W%Chg` |  | 26 Weeks |
| `Pr26WRel%Chg` |  | 26 Weeks |
| `Pr52W%Chg` |  | 52 Weeks |
| `Pr52WRel%Chg` |  | 52 Weeks |


## Price

Functions related to price EOD time series

### Benchmark Price

Historical Close price of the benchmark. Ex:

BenchClose(0)  gets the last close
BenchClose(10)  gets the close 10 bars ago.

| Factor | Params | Variant |
|--------|--------|---------|
| `BenchClose()` | barsAgo |  |
| `BenchHi()` | barsAgo |  |
| `BenchLow()` | barsAgo |  |
| `BenchOpen()` | barsAgo |  |


### Bid Ask Spread

Returns the closing spread (ask-bid) for the bar. Data is from ICE Data (formerly Interactive Data Corp).

| Factor | Params | Variant |
|--------|--------|---------|
| `Spread()` | barsAgo |  |
| `Spread_D()` | daysAgo |  |


### Price

Price ($) unadjusted for future splits. Same as Close(0)

| Factor | Params | Variant |
|--------|--------|---------|
| `Price` |  | Previous Close |
| `PricePY` |  | 1 Year Ago |


### Price Highest/Lowest

This function returns the highest value of the series within the specified lookback period. The close prices are used by default.

| Factor | Params | Variant |
|--------|--------|---------|
| `HighVal()` | period [, offset, series] |  |
| `HighValBar()` | period [, offset, series] |  |
| `LowVal()` | period [, offset, series] |  |
| `LowValBar()` | period [, offset, series] |  |
| `PriceH` |  | 52 Weeks |
| `PriceL` |  | 52 Weeks |


### Price OHLC

Historical close price 'bars' or 'trading days' ago (the length of a bar can be determined by the series used). Use negative values to peek into the future.

| Factor | Params | Variant |
|--------|--------|---------|
| `Close()` | bars [, series] | Series Dependent |
| `Close_D()` | days [, series] | Weekday |
| `Close_W()` | weeks [, series] | Weekly |
| `Hi()` | bars [, series] | Series Dependent |
| `Hi_D()` | days [, series] | Weekday |
| `Hi_W()` | weeks [, series] | Weekly |
| `Low()` | bars [, series] | Series Dependent |
| `Low_D()` | days [, series] | Weekday |
| `Low_W()` | weeks [, series] | Weekly |
| `Open()` | bars [, series] | Series Dependent |
| `Open_D()` | days [, series] | Weekday |
| `Open_W()` | weeks [, series] | Weekly |


### Price Special

Historical Close adjusted for splits even when used in the past (only availalble in the Series Tool).

NOTE: not to be used with other ratios that are point-in-time.

| Factor | Params | Variant |
|--------|--------|---------|
| `CloseAdj()` | barsAgo |  |
| `CloseExDiv()` | barsAgo |  |


## Volume

Functions related to volume EOD time series

### Average Volume

Daily average volume of the past number of bars.

| Factor | Params | Variant |
|--------|--------|---------|
| `AvgVol()` | noBars[, offset, series] | Daily Avg |
| `AvgVol10` |  | Daily Avg 2 wk |
| `AvgVol1M` |  | Daily Avg 1 Mo |
| `AvgVol3M` |  | Daily Avg 3 Mo |
| `AvgVol5` |  | Daily Avg 1 Wk |
| `AvgVol6M` |  | Daily Avg 6 Mo |
| `MedianVol()` | noBars[, offset, series] | Daily Median |
| `Vol10DAvg` |  | Daily Avg 2 Wk |
| `Vol3MAvg` |  | Monthly Average |


### Liquidity

Average daily total amount traded (price * volume) for the past number of bars. You can use the offset to calculate rising avg. For ex:

AvgDailyTot(10) > AvgDailyTot(10,10)

| Factor | Params | Variant |
|--------|--------|---------|
| `AvgDailyTot()` | noBars [, offset] |  |
| `MedianDailyTot()` | noBars [, offset] |  |
| `MinLiquidity()` | noBars [, offset] |  |
| `VolD%ShsOut` |  | Daily Avg 2 Wk |
| `VolM%ShsOut` |  | Monthly Avg 3 Mo |


### Volume

Historical volume for a day in the past.

| Factor | Params | Variant |
|--------|--------|---------|
| `Vol()` | bars [, series] | Series Dependent |
| `Vol_D()` | days [, series] | Weekday |
| `Vol_W()` | weeks [, series] | Weekly |


## Moving Average

Functions to calculate moving averages of time series.

### Exponential Moving Average

Exponential moving average of a time series. Period is in 'bars' or 'trading days ago' (can vary depending on the series you choose).

| Factor | Params | Variant |
|--------|--------|---------|
| `EMA()` | bars [, offset, series] | Series Dependent |
| `EMA_D()` | days [, offset, series] | Weekday |
| `EMA_W()` | weeks [, offset, series] | Weekly |


### Moving Avg Converge/Diverge

Moving Average Convergence/Divergence. Returns the difference between a 26-bar and a 12-bar exponential moving average.

| Factor | Params | Variant |
|--------|--------|---------|
| `MACD()` | offset [, series] |  |
| `MACDD()` | short, long [, period ,offset, series] |  |


### Moving Avg Cross Over/Under

Returns TRUE(1) when the MA(period1) is over MA(period2) and the cross happened 'bars' ago or less. Otherwise it returns FALSE(0).

type: #SMA,#EMA,#VMA, or #WMA
bars: maximum no. bars examined 1-100
period1: period for moving average 1-250
period2: period for moving average 1-250

Ex. To find all stocks whose 50 bar simple average has crossed over the 200 bar average in the last 10 bars, enter:

CrossOver(#SMA,10,50,200)=TRUE

| Factor | Params | Variant |
|--------|--------|---------|
| `CrossOver()` | type, bars, period1, period2 |  |
| `CrossUnder()` | type, bars, period1, period2 |  |


### Simple Moving Average

Simple moving average of a time series. Period is in 'bars' or 'trading days ago' (can vary depending on the series you choose).

| Factor | Params | Variant |
|--------|--------|---------|
| `SMA()` | bars [, offset, series] | Series Dependent |
| `SMA_D()` | days [, offset, series] | Weekday |
| `SMA_W()` | weeks [, offset, series] | Weekly |


### Volume weighted average

Volume weighted moving average of a time series. Period is in 'bars' or 'trading days ago' (can vary depending on the series you choose).

| Factor | Params | Variant |
|--------|--------|---------|
| `VMA()` | bars [, offset] | Series Dependent |


### Weighted moving average

Weighted moving average of a time series. Period is in 'bars' or 'trading days ago' (can vary depending on the series you choose).

| Factor | Params | Variant |
|--------|--------|---------|
| `WMA()` | bars [, offset, series] | Series Dependent |
| `WMA_D()` | days [, offset, series] | Weekday |


## Accumulation

Functions to calculate money flows in stock trading, with a particular eye toward volume analysis.

### Chaikin Accumulation Distribution

The Chaikin Accumulation Distribution Indicator is a measure of the money flowing into and out of a stock over the period

See Full Description for usage and examples

| Factor | Params | Variant |
|--------|--------|---------|
| `ChaikinAD()` | period [, offset] |  |


### Chaikin Money Flow

This indicator calculates the percentage of days in the previous lookback window that the ChaikinAD is > 0

See Full Description for usage and examples

| Factor | Params | Variant |
|--------|--------|---------|
| `ChaikinMFP()` | period, lookback[, offset] |  |


### Chaikin Trend

The ChaikinTrend Indicator is a special purpose double smoothed exponential average

| Factor | Params | Variant |
|--------|--------|---------|
| `ChaikinTrend()` | bars [, offset, increment, series] |  |


### On Balance Volume (OBV)

On Balance Volume

Returns the running total of the volume for the past 100 bars. When the security closes higher than the previous close, the day's volume is added. When is closes lower than the previous close, the day's volume is subtracted. The offset can be used to determine if the OBV trending. For example to screen for stocks whose OBV is higher than 10 bars ago enter:

OBV(0)>OBV(10)

For a better way to find trending OBV's see OBVSlopeN.

| Factor | Params | Variant |
|--------|--------|---------|
| `OBV()` | offset |  |


### On Balance Volume (OBV) Slope

Normalized rate of change of the OBV

Returns the normalized linear regression slope of bars values of OBV, or the percent change of the regression of OBV. To screen for stocks whose 10-bar OBV is increasing 20% per bar enter:

OBVSlopeN(0,10)>20

| Factor | Params | Variant |
|--------|--------|---------|
| `OBVSlopeN()` | offset, bars |  |


### Up/Down Volume Ratio

Calculates the Up/Down Volume ratio for a stock. If the ratio exceeds 0.5, it means volume on a stock's up days outweighed downside volume in the specified period. It is calculated as:

Sum Up Vol/(Sum Up Vol + Sum Down Vol)

| Factor | Params | Variant |
|--------|--------|---------|
| `UpDownRatio()` | bars, offset |  |


## Trending

Functions to analyze trend strength and direction in the market of a stock.

### Bollinger Band

Lower Bollinger band value
period: no. of bars used (typical is 20)
deviations: no. of deviations (default is 2)

| Factor | Params | Variant |
|--------|--------|---------|
| `BBLower()` | period [, deviations, offset, series] |  |
| `BBUpper()` | period [, deviations, offset, series] |  |


### Directional Movement

Returns the Average Directional movement Index as defined by Welles Wilder. An offset can be specified to find trends in the ADX.

| Factor | Params | Variant |
|--------|--------|---------|
| `ADX()` | period, offset[, series] |  |
| `DMICrossOver()` | period, bars[, series] |  |
| `DMICrossUnder()` | period, bars[, series] |  |
| `DMIMinus()` | period, offset[, series] |  |
| `DMIPlus()` | period, offset[, series] |  |


### Parabolic SAR

SAR: Parabolic SAR.

Returns the SAR(stop-and-reversal) value using an Acceleration Factor or 0.02 and a maximum Acceleration of 0.2.To find stocks trading above the SAR enter:

Close(0)>SAR

| Factor | Params | Variant |
|--------|--------|---------|
| `SAR` |  |  |


### Price Regression End Value

Returns the ending value of a Regression Line of the prices (incl div)

| Factor | Params | Variant |
|--------|--------|---------|
| `PrcRegEst()` | bars [, series] | Series Dependent |
| `PrcRegEst_W()` | bars [, series] | Weekly |
| `PrcRegEst10` |  | 10 Bars |
| `PrcRegEst10W` |  | 10 Weeks |
| `PrcRegEst20` |  | 20 Bars |
| `PrcRegEst20W` |  | 20 Weeks |
| `PrcRegEst50` |  | 50 Bars |
| `PrcRegEst50W` |  | 50 Weeks |


### Rate of Change (ROC)

Rate of Change.

| Factor | Params | Variant |
|--------|--------|---------|
| `ROC()` | bars[, offset, series] |  |


## Pattern

Gap Up, Gap Down.

### Gap Down

This function returns TRUE (1) when a stock has a Gap Down pattern in the period specified by the 'bars' parameters, with the start bar being specified by 'offset'.

| Factor | Params | Variant |
|--------|--------|---------|
| `GapDown()` | GapPct, VolPct, bars, offset |  |


### Gap Up

This function returns TRUE (1) when a stock has a Gap Up pattern in the period specified by the 'bars' parameters, with the start bar being specified by 'offset'.

| Factor | Params | Variant |
|--------|--------|---------|
| `GapUp()` | GapPct, VolPct, bars, offset |  |


## Oscillators

Functions that either return a positive or a negative condition at any given time.

### Commodity Channel Index

Commodity Channel Index.

| Factor | Params | Variant |
|--------|--------|---------|
| `CCI()` | bars[, offset, series] |  |


### Flip Flop

Returns TRUE or FALSE depending on the last threshold that was exceeded

| Factor | Params | Variant |
|--------|--------|---------|
| `FlipFlop()` | series, on_value, off_value[, initial_state] |  |


### Momentum

Measures the amount that a security's closing price has changed over a given time span.

absolute = FALSE (default) calculates as 100*Close(0)/Close(bars)
absolute = TRUE calculates as Close(0)-Close(bars)

See Full Description for details.

| Factor | Params | Variant |
|--------|--------|---------|
| `Momentum()` | bars[, offset, absolute] |  |


### Relative Strength Indicator (RSI)

Welles Wilder's Relative Strength Index. Period is in 'bar' or 'trading days' (can depend on the series you specify)

| Factor | Params | Variant |
|--------|--------|---------|
| `RSI()` | period [, offset, series] | Series Dependent |
| `RSI_D()` | days [, offset, series] | Weekday |
| `RSI_W()` | weeks [, offset, series] | Week |


### Stochastic Oscillator

Returns the Stochastic %D value

| Factor | Params | Variant |
|--------|--------|---------|
| `StochD()` | period ,smoothK , smoothD [, offset, series] |  |
| `StochK()` | period [, smoothK, offset, series] |  |


### Ultimate Oscillator

Ultimate Oscillator.

Returns the weighted sum of three oscillators of different time periods as defined by Larry Williams. An offset can be specified to find trends in the ULTOSC to find divergences with the price.

| Factor | Params | Variant |
|--------|--------|---------|
| `ULTOSC()` | offset |  |


## Volatility

Quantifications of the variability of a time series.

### Average Percent Change

Calculates the average of the percentage moves for selected period. To calculate the average of the past 20 weeks enter PctAvg(20,5). Note: using a bar length of 5 returns weekly percentage moves if there are no holidays.

| Factor | Params | Variant |
|--------|--------|---------|
| `PctAvg()` | samples, bars[, offset, min_samples, annualize] |  |


### Average True Range

Returns the Average True Range as defined by Welles Wilder over the specified period.

| Factor | Params | Variant |
|--------|--------|---------|
| `ATR()` | bars [, offset, series] |  |


### Average True Range Normalized

Returns ATR as a percentage of the closing price. ATRN provides a better way to compare stocks with different price magnitude.

| Factor | Params | Variant |
|--------|--------|---------|
| `ATRN()` | bars [, offset, series] |  |


### Beta

Returns Beta using up to 1 year of weekly returns of the stock and the country's main benchmark.

| Factor | Params | Variant |
|--------|--------|---------|
| `Beta1Y` |  | 1 Year |
| `Beta3Y` |  | 3 Years |
| `Beta5Y` |  | 5 Years |
| `BetaFunc()` | period, samples[, min_samples, offset, series] |  |


### Correlation coefficient

This function returns the correlation coefficient between the specified series

| Factor | Params | Variant |
|--------|--------|---------|
| `Correl()` | period , samples , series [, series2] |  |


### Sharpe Ratio

Returns a sharpe-like ratio. Unlike the normal Sharpe ratio, it is not adjusted for the risk-free return.

| Factor | Params | Variant |
|--------|--------|---------|
| `Sharpe()` | range[, bars, offset] |  |
| `Sharpe1Y` |  | 1 Year |
| `Sharpe2Y` |  | 2 Years |


### Sortino Ratio

Returns a sortino-like ratio. Unlike the normal Sortino ratio, it is not adjusted for the risk-free return.

range: total number of bars used
bars: no. bars used for the returns (default=5)
offset: offset in bars

| Factor | Params | Variant |
|--------|--------|---------|
| `Sortino()` | range[, bars, offset] |  |
| `Sortino1Y` |  | 1 Year |
| `Sortino2Y` |  | 2 Years |


### Standard Deviation (Volatility)

Calculates the standard deviation of the percentage moves of the closing prices. For example to calculate the SD of 50  weekly percentage moves enter: PctDev(50,5)

| Factor | Params | Variant |
|--------|--------|---------|
| `PctDev()` | samples, bars[, offset, min_samples, annualize] |  |
| `TRSD1YD` |  | 1 Year |
| `TRSD30D` |  | 30 Days |
| `TRSD3YD` |  | 3 Years |
| `TRSD3YM` |  | 3 Years |
| `TRSD5YD` |  | 5 Years |
| `TRSD5YM` |  | 5 Years |
| `TRSD60D` |  | 60 Days |
| `TRSD90D` |  | 90 Days |

