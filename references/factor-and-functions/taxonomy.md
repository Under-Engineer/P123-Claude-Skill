# Taxonomy

ETF classifications.

## ETF Asset Class

ETFAssetClass returns the ETF Asset Class. 

For example to eliminate all currency ETFs enter:
ETFAssetClass !=  CURR

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFAssetClass` |  |  |
| `ETFAssetClassSet()` | x1[, x2..x30] |  |


## ETF Country

ETFCountry returns the ETF Country. 

For example to eliminate all chinese ETFs enter:
ETFCountry !=  CHINA

NOTE: ETFs that span multiple countries are set to MULTICTRY.

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFCountry` |  |  |
| `ETFCountrySet()` | x1[, x2..x30] |  |


## ETF Family

ETFFamily returns the ETF Family. 

For example to eliminate all iShares ETFs enter:
ETFFamily !=  ISHARES

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFFamily` |  |  |
| `ETFFamilySet()` | x1[, x2..x30] |  |


## ETF Method

ETFMethod returns the ETF Method. 

For example to return only  short ETFs enter:
ETFMethod =  LEVSHORT or ETFMethod = STANSHORT

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFMethod` |  |  |
| `ETFMethodSet()` | x1[, x2..x30] |  |


## ETF Region

ETFRegion returns the ETF Region. 

For example to eliminate all emerging markets ETFs enter:
ETFRegion !=  EMERG

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFRegion` |  |  |
| `ETFRegionSet()` | x1[, x2..x30] |  |


## ETF Sector

ETFSector returns the ETFSector. 

For example to eliminate all financial ETFs enter:
ETFSector !=  FINANCIAL

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFSector` |  |  |
| `ETFSectorSet()` | x1[, x2..x30] |  |


## ETF Size

ETFSize returns the ETF Size. 

For example to eliminate all smallcap ETFs enter:
ETFSize !=  ETF_SMALLCAP

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFSize` |  |  |
| `ETFSizeSet()` | x1[, x2..x30] |  |


## ETF Style

ETFStyle returns the ETF Style. 

For example to eliminate all value ETFs enter:
ETFStyle !=  VALUE

| Factor | Params | Variant |
|--------|--------|---------|
| `ETFStyle` |  |  |
| `ETFStyleSet()` | x1[, x2..x30] |  |

