# Misc

Functions that do not fit into any other category.

## Time Series IDs

Series IDs that can be used as the series parameters in functions, or in the charts section. For example you can retrieve the latest value of the SP500 Index with:<br><br>Close(0,$SP500)<br><br>See the Full Description of each ID for more examples.

### S&P 500 IDs

SP500 Risk Premium (weekly)

| Factor | Params | Variant |
|--------|--------|---------|
| `#SPRPBlend` | series | Weekly |
| `#SPYieldBlend` | series | Weekly |
| `#SPEPSCNY` | series | Weekly |
| `#SPEPSQ` | series | Weekly |
| `#SPEPSTTM` | series | Weekly |


### Index Tickers - Major

S&P 400 Mid

| Factor | Params | Variant |
|--------|--------|---------|
| `$MID` | series |  |
| `$RUA` | series |  |
| `$RUI` | series |  |
| `$RUT` | series |  |
| `$SML` | series |  |
| `$SP500` | series |  |
| `$SP500EQ` | series |  |
| `$SPALL` | series |  |


### Index Tickers - Specialty

Dow Jones

| Factor | Params | Variant |
|--------|--------|---------|
| `$DJIA` | series |  |
| `$MIDPG` | series |  |
| `$MIDPV` | series |  |
| `$NASDAQ` | series |  |
| `$NASDAQ100` | series |  |
| `$SMLPG` | series |  |
| `$SMLPV` | series |  |
| `$SP500PG` | series |  |
| `$SP500PV` | series |  |
| `$SPALLCND` | series |  |
| `$SPALLCNS` | series |  |
| `$SPALLENG` | series |  |
| `$SPALLEUT` | series |  |
| `$SPALLFIN` | series |  |
| `$SPALLGLD` | series |  |
| `$SPALLHEA` | series |  |
| `$SPALLHEQ` | series |  |
| `$SPALLIND` | series |  |
| `$SPALLINT` | series |  |
| `$SPALLMAT` | series |  |
| `$SPALLPBL` | series |  |
| `$SPALLPG` | series |  |
| `$SPALLPV` | series |  |
| `$SPALLTCM` | series |  |
| `$SPALLUTL` | series |  |
| `$VIX` | series |  |


### Misc IDs

Current benchmark closing prices (daily)

| Factor | Params | Variant |
|--------|--------|---------|
| `#Bench` | series |  |
| `#Equity` | series |  |
| `#TNX` | series |  |


### Price IDs

Stock closing prices (daily)

| Factor | Params | Variant |
|--------|--------|---------|
| `#Close` | series |  |
| `#High` | series |  |
| `#Low` | series |  |
| `#Open` | series |  |


## Macro Series IDs (Adjusted)

FRED macro series that are seasonally adjusted.

### Macro - Other Economic Activity

Debt as Percent of GDP (quarterly)

Corresponding FRED id=GFDEGDQ188S

| Factor | Params | Variant |
|--------|--------|---------|
| `##DBTGDP` | series | Quarterly |
| `##DOMINV` | series | Quarterly |
| `##PCE` | series | Monthly |
| `##RPCE` | series | Monthly |
| `##SAVING` | series | Monthly |
| `##SURPLUS` | series | Annual |
| `##USSLIND` | series | Monthly |


### Macro - Delinquency Rate

Delinquency Rate On Credit Card Loans, All Commercial Banks (quarterly)

Corresponding FRED id=DRCCLACBS

| Factor | Params | Variant |
|--------|--------|---------|
| `##DELINQCC` | series | Quarterly |
| `##DELINQMORT` | series | Quarterly |


### Macro - GDP/GNP

Gross National Product (quarterly)

Corresponding FRED id=GNP

| Factor | Params | Variant |
|--------|--------|---------|
| `##GNP` | series | Quarterly |
| `##RGDP` | series | Quarterly |


### Macro - Income

Household Debt Service Payments as a Percent of Disposable Personal Income (quarterly)

Corresponding FRED id=TDSP

| Factor | Params | Variant |
|--------|--------|---------|
| `##HDEBTSERV` | series | Quarterly |
| `##RDISPINC` | series | Monthly |
| `##RINCPERCAP` | series | Monthly |
| `##RMINCOME` | series | Annual |


### Macro - Labor Force

Civilian Labor Force (monthly)

Corresponding FRED id=CLF16OV

| Factor | Params | Variant |
|--------|--------|---------|
| `##CIVLABOR` | series | Monthly |
| `##LABORPARTIC` | series | Monthly |
| `##NONFARMEMPL` | series | Monthly |
| `##POPUL` | series | Monthly |
| `##UNWANT` | series | Monthly |


### Macro - Manufacturing

Ratio of Total Inventories to Shipments for All Manufacturing Industries (monthly)

Corresponding FRED id=AMTMUS

| Factor | Params | Variant |
|--------|--------|---------|
| `##INV2SHIP` | series | Monthly |
| `##ORDERSCAP` | series | Monthly |
| `##ORDERSDUR` | series | Monthly |
| `##ORDERSUNFILL` | series | Monthly |
| `##WAGES` | series | Monthly |


### Macro - Money, M1, M2

Monetary Base; Total (monthly)

Corresponding FRED id=BOGMBASE

| Factor | Params | Variant |
|--------|--------|---------|
| `##ADJMBASE` | series | Monthly |
| `##M1` | series | Monthly |
| `##M2` | series | Monthly |
| `##USCURRACCT` | series | Quarterly |
| `##VELM1` | series | Quarterly |
| `##VELM2` | series | Quarterly |


### Macro - Other Business Activity

Capacity Utilization: Total Industry (monthly)

Corresponding FRED id=TCU

| Factor | Params | Variant |
|--------|--------|---------|
| `##CAPUTIL` | series | Monthly |
| `##CONSTR` | series | Monthly |
| `##HSTARTS` | series | Monthly |
| `##INDPRO` | series | Monthly |
| `##INV2SLS` | series | Monthly |
| `##INVTOT` | series | Monthly |
| `##SALESRET` | series | Monthly |
| `##SALESRETFD` | series | Monthly |


### Macro - Price Index, CPI, PPI, HPI

CPI All Urban Consumers: All Items (monthly)

Corresponding FRED id=CPIAUCSL

| Factor | Params | Variant |
|--------|--------|---------|
| `##CPI` | series | Monthly |
| `##HPRICES` | series | Monthly |
| `##PPI` | series | Monthly |


### Macro - Sentiment

Smoothed U.S. Recession Probabilities (monthly)

Corresponding FRED id=RECPROUSM156N

| Factor | Params | Variant |
|--------|--------|---------|
| `##RECPROB` | series | Monthly |
| `##UMCSENT` | series | Monthly |
| `##INFLEXP` | series | Monthly |


### Macro - Unemployment

Continued Claims (Insured Unemployment) (weekly)

Corresponding FRED id=CCSA

| Factor | Params | Variant |
|--------|--------|---------|
| `##CLAIMSCONTINUE` | series | Weekly |
| `##CLAIMSNEW` | series | Weekly |
| `##UNDURATION` | series | Monthly |
| `##UNRATE` | series | Monthly |
| `##UNTEEN` | series | Monthly |
| `##UNTOT` | series | Monthly |


### Macro - Vehicle, Automobile

Auto Inventory/Sales Ratio (monthly)

Corresponding FRED id=AISRSA

| Factor | Params | Variant |
|--------|--------|---------|
| `##INV2SLSAUTO` | series | Monthly |
| `##PRODAUTO` | series | Monthly |
| `##SALESALLVEH` | series | Monthly |
| `##SALESAUTO` | series | Monthly |


## Macro Series IDs (Unadjusted)

FRED macro series that are not seasonally adjusted.

### Macro - Currency

Nominal Broad U.S. Dollar Index (daily)

Corresponding FRED id=DTWEXBGS

| Factor | Params | Variant |
|--------|--------|---------|
| `##NBDI` | series | Weekday |
| `##RBDI` | series | Monthly |


### Macro - Interbank Rate

3-Month Interbank Rate for Canada (monthly)

Corresponding FRED id=IR3TIB01CAM156N

| Factor | Params | Variant |
|--------|--------|---------|
| `##CAB3MO` | series | Monthly |
| `##EUB3MO` | series | Monthly |
| `##GBB3MO` | series | Monthly |
| `##NOB3MO` | series | Monthly |
| `##PLB3MO` | series | Monthly |
| `##SEB3MO` | series | Monthly |


### Macro - Interest, Mortgage, Prime, TED

90-Day Average SOFR (daily)

Corresponding FRED id=SOFR90DAYAVG

| Factor | Params | Variant |
|--------|--------|---------|
| `##SOFR3MO` | series | Weekday |
| `##USR10YR` | series | Monthly |
| `##FEDFUNDS` | series | Weekday |
| `##MORT30Y` | series | Weekly |
| `##PRIME` | series | Monthly |


### Macro - Treasury notes (T-notes)

10-Year Government Bond Yield for Canada (monthly)

Corresponding FRED id=IRLTLT01CAM156N

| Factor | Params | Variant |
|--------|--------|---------|
| `##CAT10YR` | series | Monthly |
| `##CHT10YR` | series | Monthly |
| `##EUT10YR` | series | Monthly |
| `##GBT10YR` | series | Monthly |
| `##UST6MO` | series | Weekday |
| `##UST2YR` | series | Weekday |
| `##UST3YR` | series | Weekday |
| `##UST5YR` | series | Weekday |
| `##UST7YR` | series | Weekday |
| `##UST10YR` | series | Weekday |


### Macro - FX Rates

USD to AUD

| Factor | Params | Variant |
|--------|--------|---------|
| `#USDAUD` | series |  |
| `#USDBAM` | series |  |
| `#USDBGN` | series |  |
| `#USDCAD` | series |  |
| `#USDCHF` | series |  |
| `#USDCZK` | series |  |
| `#USDDKK` | series |  |
| `#USDEUR` | series |  |
| `#USDGBP` | series |  |
| `#USDHKD` | series |  |
| `#USDHRK` | series |  |
| `#USDHUF` | series |  |
| `#USDILS` | series |  |
| `#USDISK` | series |  |
| `#USDJPY` | series |  |
| `#USDLVL` | series |  |
| `#USDMKD` | series |  |
| `#USDMXN` | series |  |
| `#USDNOK` | series |  |
| `#USDNZD` | series |  |
| `#USDPLN` | series |  |
| `#USDRON` | series |  |
| `#USDRSD` | series |  |
| `#USDRUB` | series |  |
| `#USDSEK` | series |  |
| `#USDSGD` | series |  |
| `#USDSKK` | series |  |
| `#USDTRY` | series |  |
| `#USDUAH` | series |  |
| `#USDZAR` | series |  |


### Macro - Corporate Bonds

BofA Merrill Lynch US Corporate AAA Effective Yield© (daily)

Corresponding FRED id=BAMLC0A1CAAAEY

| Factor | Params | Variant |
|--------|--------|---------|
| `##CORPAAA` | series | Weekday |
| `##CORPB` | series | Weekday |
| `##CORPBB` | series | Weekday |
| `##CORPBBB` | series | Weekday |
| `##CORPBBBOAS` | series | Weekday |
| `##CORPBBOAS` | series | Weekday |
| `##CORPJNK` | series | Weekday |


### Macro - Oil, Gold Price

Crude Oil Prices: West Texas Intermediate (WTI) - Cushing, OK (daily)

Corresponding FRED id=DCOILWTICO

| Factor | Params | Variant |
|--------|--------|---------|
| `##OIL` | series | Weekday |


### Macro - Stress Index

St. Louis Fed Financial Stress Index© (weekly)

Corresponding FRED id=STLFSI4

| Factor | Params | Variant |
|--------|--------|---------|
| `##STRESS` | series | Weekly |


### Macro - Treasury bills (T-bills)

1-Month Treasury Constant Maturity Rate (USD) (daily)

Corresponding FRED id=DGS1MO

| Factor | Params | Variant |
|--------|--------|---------|
| `##UST1MO` | series | Weekday |
| `##UST3MO` | series | Weekday |
| `##UST1YR` | series | Weekday |


### Macro - Vacancy Rates

Home Vacancy Rate for the United States (annual)

Corresponding FRED id=USHVAC

| Factor | Params | Variant |
|--------|--------|---------|
| `##HVACANCY` | series | Annual |
| `##RVACANCY` | series | Annual |


### Macro - Treasury bonds (T-bonds)

20-Year Treasury Constant Maturity Rate (USD) (daily)

Corresponding FRED id=DGS20

| Factor | Params | Variant |
|--------|--------|---------|
| `##UST20YR` | series | Weekday |
| `##UST30YR` | series | Weekday |


### Compustat Macro - TO BE DEPRECATED

20-Year Treasury Yield (monthly)

| Factor | Params | Variant |
|--------|--------|---------|
| `#BOND20YR` | series | Monthly |
| `#BOND30YR` | series | Monthly |
| `#CABGDP2` | series | Quarterly* |
| `#CPI` | series | Monthly |
| `#EMPLOY` | series | Monthly |
| `#FEDFUNDS` | series | Monthly |
| `#GDP` | series | Quarterly* |
| `#HOUSE` | series | Monthly |
| `#M1` | series | Monthly |
| `#M2` | series | Monthly |
| `#NOTE10YR` | series | Monthly |
| `#NOTE2YR` | series | Monthly |
| `#NOTE3YR` | series | Monthly |
| `#NOTE5YR` | series | Monthly |
| `#NOTE7YR` | series | Monthly |
| `#POPT` | series | Annual* |
| `#PPI` | series | Monthly |
| `#PRIME` | series | Monthly |
| `#RTLSALES` | series | Monthly |
| `#TBILL12M` | series | Monthly |
| `#TBILL3M` | series | Monthly |
| `#TBILL6M` | series | Monthly |
| `#UNEMP` | series | Monthly |


## Group

Functions that perform calculations on groups of stocks or that identify individual stocks.

### Company Name

Returns 1(TRUE) if the company name is in the list, 0 (FALSE) otherwise. You can also use wildcards * to match any string or ? for any character

| Factor | Params | Variant |
|--------|--------|---------|
| `CoName()` | "name" |  |


### Stock is in Custom List

Returns 1 if the stock is in your custom list, 0 otherwise. To enter a custom list go to TOOLS->Lists->Custom. Ex: to only buy stocks in your list "MyList" enter the following Buy rule:

InList("MyList")

| Factor | Params | Variant |
|--------|--------|---------|
| `InList()` | "MyListName" |  |


### Unique ID Odd or Even

Returns 1 (TRUE) if the internal ID of the stock or ETF is Even, 0 (FALSE) otherwise. Can be used for data-mining to create two samples from the universe.

| Factor | Params | Variant |
|--------|--------|---------|
| `EvenID` |  |  |


### Universe filter

Returns 1 if the stock is in the universe, 0 otherwise. Ex: to only buy S&P 500 stocks enter the following Buy rule:

Universe(SP500)

To see all universes click on 'Full Description'

| Factor | Params | Variant |
|--------|--------|---------|
| `Universe()` | uname |  |


## RBICS Codes

RBICS codes that can be used in the RBICS() function.

### Business Services

10 - Business Services

| Factor | Params | Variant |
|--------|--------|---------|
| `BIZSVCE` | rcode |  |
| `BIZSVCESS` | rcode |  |
| `MKTINGPRINTING` | rcode |  |
| `ADVERTISING` | rcode |  |
| `PRINTING` | rcode |  |
| `PROSVCE` | rcode |  |
| `ADMINSVCE` | rcode |  |
| `CONSULTING` | rcode |  |
| `PROSVCEOTHER` | rcode |  |
| `BIZSUPPORT` | rcode |  |
| `FACILSVCE` | rcode |  |
| `SECURITYSVCE` | rcode |  |
| `WASTEMGMT` | rcode |  |
| `WASTECOLLECTION` | rcode |  |
| `HAZMAT` | rcode |  |
| `WASTESVCE` | rcode |  |
| `WASTEWATER` | rcode |  |
| `ENVISVCE` | rcode |  |
| `DEMOSVCE` | rcode |  |


### Consumer Cyclicals

20 - Consumer Cyclicals

| Factor | Params | Variant |
|--------|--------|---------|
| `CYCLICALS` | rcode |  |
| `CONSUMERGOODS` | rcode |  |
| `APPARELPRODUCTS` | rcode |  |
| `ACCESSORIESMFR` | rcode |  |
| `CLOTHINGMFR` | rcode |  |
| `APPARELMFR` | rcode |  |
| `LEISURE` | rcode |  |
| `LEISUREOTHER` | rcode |  |
| `RECREATIONALGOODS` | rcode |  |
| `SPORTINGGOODS` | rcode |  |
| `APPLIANCESFURN` | rcode |  |
| `RETAILMISC` | rcode |  |
| `AUTORETAIL` | rcode |  |
| `AUTOSVCE` | rcode |  |
| `AUTOSALES` | rcode |  |
| `AUTOPARTSSALESRENT` | rcode |  |
| `RETAILOTHER` | rcode |  |
| `AUCTION` | rcode |  |
| `GASSTATION` | rcode |  |
| `OFFICESUPPLY` | rcode |  |
| `PETS` | rcode |  |
| `RETAILSOFTW` | rcode |  |
| `EVSTATION` | rcode |  |
| `CANNABISRETAIL` | rcode |  |
| `HOMEBUILDMANUF` | rcode |  |
| `HOMEBUILD` | rcode |  |
| `MFRBUILDING` | rcode |  |
| `VEHICLESS` | rcode |  |
| `VEHICLE` | rcode |  |
| `AUTOPARTSMFR` | rcode |  |
| `AUTOMFR` | rcode |  |
| `CONSUMERRETAIL` | rcode |  |
| `APPARELRETAIL` | rcode |  |
| `ACCESSORIESRETAIL` | rcode |  |
| `CLOTHINGACCESSORIESRETAIL` | rcode |  |
| `CLOTHINGRETAIL` | rcode |  |
| `SHOES` | rcode |  |
| `ELECTRONICSENTRETAIL` | rcode |  |
| `ELECTRONICSRETAIL` | rcode |  |
| `ENTRETAIL` | rcode |  |
| `ELECTRONICSENTMIXRETAIL` | rcode |  |
| `HOMEIMPROVE` | rcode |  |
| `BUILDINGMAT` | rcode |  |
| `STOREFURNITURE` | rcode |  |
| `HOMEIMPROV` | rcode |  |


### Consumer Non-Cyclicals

50 - Consumer Non-Cyclicals

| Factor | Params | Variant |
|--------|--------|---------|
| `NONCYCLICAL` | rcode |  |
| `STAPLESRETAIL` | rcode |  |
| `FOODDRINKRETAIL` | rcode |  |
| `STOREFOOD` | rcode |  |
| `FOODDRINKRETAILGEN` | rcode |  |
| `GROCERY` | rcode |  |
| `RETAILDISTRIB` | rcode |  |
| `GENMERCH` | rcode |  |
| `STOREDEPT` | rcode |  |
| `STOREDISC` | rcode |  |
| `MERCHRETAIL` | rcode |  |
| `OFFPRICERETAIL` | rcode |  |
| `WAREHOUSECLUB` | rcode |  |
| `PERSONALCARERETAIL` | rcode |  |
| `PERSONALCARERETAILGEN` | rcode |  |
| `PERSONALCARERETAILOTHER` | rcode |  |
| `PHARMACY` | rcode |  |
| `FOODPRODUCTION` | rcode |  |
| `AGRICULTURE` | rcode |  |
| `ANIMAL` | rcode |  |
| `CROP` | rcode |  |
| `AGRICDIV` | rcode |  |
| `AGRICSUPPORT` | rcode |  |
| `FOODDRINKMFR` | rcode |  |
| `BEVERAGE` | rcode |  |
| `FOOD` | rcode |  |
| `FOODDRINKMFRGEN` | rcode |  |
| `TOBACCO` | rcode |  |
| `CIGARETTE` | rcode |  |
| `TOBACCOMFRGEN` | rcode |  |
| `TOBACCOPRODUCT` | rcode |  |
| `ECIGARETTE` | rcode |  |
| `CANNABIS` | rcode |  |
| `PRODHOUSESUBSECT` | rcode |  |
| `APPLIANCESTOOLS` | rcode |  |
| `APPLIANCESTOOLSDIV` | rcode |  |
| `APPLIANCESSMALL` | rcode |  |
| `PRODHOUSEIND` | rcode |  |
| `BABYMFR` | rcode |  |
| `PRODHOUSEDIV` | rcode |  |
| `HOMEOFFICEFURNMFR` | rcode |  |
| `PERSONALCAREPRODUCT` | rcode |  |
| `ABSORBENT` | rcode |  |
| `COSMETICS` | rcode |  |
| `FRAGRANCE` | rcode |  |
| `PERSONALCAREGEN` | rcode |  |
| `HAIRCARE` | rcode |  |
| `CLEANING` | rcode |  |
| `SANITARY` | rcode |  |
| `SKINCARE` | rcode |  |
| `HOUSESVCESS` | rcode |  |
| `HOUSESVCE` | rcode |  |
| `EDUCATION` | rcode |  |
| `PERSONALSVCE` | rcode |  |


### Consumer Services

15 - Consumer Services

| Factor | Params | Variant |
|--------|--------|---------|
| `CONSUMERSVCE` | rcode |  |
| `HOSPITALITYSS` | rcode |  |
| `HOSPITALITY` | rcode |  |
| `HOTEL` | rcode |  |
| `ARTSENT` | rcode |  |
| `FOODDRINKSVCE` | rcode |  |
| `RESTAURANT` | rcode |  |
| `TRAVEL` | rcode |  |
| `MEDIAPUBSS` | rcode |  |
| `MEDIAPUB` | rcode |  |
| `BROADCAST` | rcode |  |
| `ENTERTAINMENT` | rcode |  |
| `BOOKS` | rcode |  |


### Energy

25 - Energy

| Factor | Params | Variant |
|--------|--------|---------|
| `ENERGY` | rcode |  |
| `UPSTREAMENERGY` | rcode |  |
| `COAL` | rcode |  |
| `COALAMER` | rcode |  |
| `COALASIA` | rcode |  |
| `COALINTL` | rcode |  |
| `URANIUMRADIUMVANADIUM.XX1` | rcode |  |
| `RADIUMVANADIUM` | rcode |  |
| `URANIUM` | rcode |  |
| `COALSTREAMING` | rcode |  |
| `FOSSILFUEL` | rcode |  |
| `FOSSILFUELAMER` | rcode |  |
| `FOSSILFUELINT.XX1` | rcode |  |
| `FOSSILFUELOTHER` | rcode |  |
| `OILGASSUPPORT` | rcode |  |
| `OILGASTRANSPORT` | rcode |  |
| `OILGASFIELD` | rcode |  |
| `OILGASOPER` | rcode |  |
| `DOWNMIDSTREAMENERGY` | rcode |  |
| `DOWNSTREAMENERGY` | rcode |  |
| `LPGPROPANE` | rcode |  |
| `REFINERIES` | rcode |  |
| `MIDSTREAMENERGY` | rcode |  |
| `NATGASPIPELINE` | rcode |  |
| `PIPELINEOTHER` | rcode |  |
| `PETROLPIPELINE` | rcode |  |
| `GATHERPROCESSSVCE` | rcode |  |
| `OILGASINTEGSS` | rcode |  |
| `OILGASINTEG` | rcode |  |


### Finance

30 - Finance

| Factor | Params | Variant |
|--------|--------|---------|
| `FINANCIAL` | rcode |  |
| `BANKS` | rcode |  |
| `BANKSINTL` | rcode |  |
| `BANKSAMEREXUS` | rcode |  |
| `BANKSASIA` | rcode |  |
| `BANKSEUROPE` | rcode |  |
| `BANKSMULTINAT` | rcode |  |
| `BANKSMORTG` | rcode |  |
| `BANKSUSA` | rcode |  |
| `BANKSCOMMERCIAL` | rcode |  |
| `SAVINGSLOAN` | rcode |  |
| `CREDITUNIONS` | rcode |  |
| `BANKSINTERNET` | rcode |  |
| `INSURANCESS` | rcode |  |
| `INSURANCE` | rcode |  |
| `INSBROKER` | rcode |  |
| `INSLIFEHEALTH` | rcode |  |
| `INSPROPCAS` | rcode |  |
| `INSRE` | rcode |  |
| `INSDIV` | rcode |  |
| `INVESTSVCESS` | rcode |  |
| `INVESTSVCE` | rcode |  |
| `ASSETMGMT` | rcode |  |
| `INVESTBANK` | rcode |  |
| `INVESTHOLDING` | rcode |  |
| `SECURITIES` | rcode |  |
| `INVESTDIV` | rcode |  |
| `REALESTATE` | rcode |  |
| `HOMEBUILDMANUF.XX1` | rcode |  |
| `HOMEBUILD.XX1` | rcode |  |
| `MFRBUILDING.XX1` | rcode |  |
| `REALESTATESVCE` | rcode |  |
| `REALESTATESVCEOTHER` | rcode |  |
| `PROPERTY` | rcode |  |
| `REIT` | rcode |  |
| `REITDIV` | rcode |  |
| `REITEQUITY` | rcode |  |
| `REITMORTG` | rcode |  |
| `FINSVCE` | rcode |  |
| `FINSPECIAL` | rcode |  |
| `FINCOMMSVCE` | rcode |  |
| `FINCONSUMERSVCE` | rcode |  |
| `FINSOFTW` | rcode |  |


### Healthcare

35 - Healthcare

| Factor | Params | Variant |
|--------|--------|---------|
| `HEALTHCARE` | rcode |  |
| `BIOPHARMA` | rcode |  |
| `BIOPHARMANONSYS` | rcode |  |
| `INFECTIOUS` | rcode |  |
| `ONCOLOGY` | rcode |  |
| `BIOPHARMAOTHER` | rcode |  |
| `ALLERGIES` | rcode |  |
| `PAINMGMT` | rcode |  |
| `SURGICAL` | rcode |  |
| `TOXICOLOGY` | rcode |  |
| `TRANSPLANTATION` | rcode |  |
| `WEIGHTMGMT` | rcode |  |
| `BIOPHARMADIV` | rcode |  |
| `BIOPHARMASYS` | rcode |  |
| `CARDIOVASCULAR` | rcode |  |
| `DERMATOLOGY` | rcode |  |
| `DIGESTIVE` | rcode |  |
| `ENDOCRINOLOGY` | rcode |  |
| `HEMATOLOGY` | rcode |  |
| `IMMUNOLOGY` | rcode |  |
| `MUSCULOSKELETAL` | rcode |  |
| `NEUROLOGY` | rcode |  |
| `OBSTETRICS` | rcode |  |
| `OPHTHALMOLOGY` | rcode |  |
| `RESPIRATORY` | rcode |  |
| `UROLOGY` | rcode |  |
| `HCARESVCE` | rcode |  |
| `HCARESUPPORT` | rcode |  |
| `HPLAN` | rcode |  |
| `HCAREADMIN` | rcode |  |
| `HCAREDISTRIB` | rcode |  |
| `HCARESUPPORTOTHER` | rcode |  |
| `PATIENTCARE` | rcode |  |
| `ACUTECARE` | rcode |  |
| `AMBULANCE` | rcode |  |
| `LTCARE` | rcode |  |
| `MULTIDELIVCARE` | rcode |  |
| `AMBULANCEOTHER` | rcode |  |
| `HCAREMISC` | rcode |  |
| `NUTRITION` | rcode |  |
| `OUTSOURCEDBIOMED` | rcode |  |
| `OUTSOURCEDDRUG` | rcode |  |
| `HCARESCIPRODUCTS` | rcode |  |
| `VETERINARY` | rcode |  |
| `HCARESVCEDIV` | rcode |  |
| `HCAREOUTSOURCE` | rcode |  |
| `HCARECONTRACTMFR` | rcode |  |
| `HCARECONTRACTRESEARCH` | rcode |  |
| `HCAREDEV` | rcode |  |
| `HCAREEQUIP` | rcode |  |
| `HCAREDIAGNOSTICS` | rcode |  |
| `DIAGNOSTIC` | rcode |  |
| `DRUGDELIV` | rcode |  |
| `MEDDEVICESGEN` | rcode |  |
| `SYSTEMSPECIFIC` | rcode |  |
| `MEDDEVICESDIV` | rcode |  |
| `MEDDEVICESOTHER` | rcode |  |
| `MEDSUPPLIES` | rcode |  |
| `MEDDEVICESSPECIAL` | rcode |  |


### Industrials

40 - Industrials

| Factor | Params | Variant |
|--------|--------|---------|
| `INDUSTRIAL` | rcode |  |
| `INDMFR` | rcode |  |
| `AERODEF` | rcode |  |
| `AEROSPACEEQUIP` | rcode |  |
| `DEF` | rcode |  |
| `AERODEFDIV` | rcode |  |
| `ELECTREQUIP` | rcode |  |
| `COMMELECTRIC` | rcode |  |
| `ELECTREQUIPOTHER` | rcode |  |
| `POWERGEN` | rcode |  |
| `MACHINE` | rcode |  |
| `CONTROLEQUIP` | rcode |  |
| `AUTOMATIONEQUIP` | rcode |  |
| `MACHINEPARTS` | rcode |  |
| `CONSTRUCTIONMACHINE` | rcode |  |
| `MACHINEOTHER` | rcode |  |
| `TOOLS` | rcode |  |
| `TRANSPORTEQUIP` | rcode |  |
| `TRANSPORTEQUIPCML` | rcode |  |
| `TRANSPORTEQUIPGEN` | rcode |  |
| `INDSVCE` | rcode |  |
| `TRAINTRUCK` | rcode |  |
| `AIRWATER` | rcode |  |
| `TRAINTRUCKGEN` | rcode |  |
| `TRAINTRUCKOP` | rcode |  |
| `INTERMODAL` | rcode |  |
| `DELIVERY` | rcode |  |
| `EXPRESS` | rcode |  |
| `DELIVERYGEN` | rcode |  |
| `LOGISTICS` | rcode |  |
| `INDLDIST` | rcode |  |
| `EQUIPDISTRIB` | rcode |  |
| `MATDISTRIB` | rcode |  |
| `INDLDIVDISTRIB` | rcode |  |
| `BUILDINGMATDIST` | rcode |  |
| `FACIL` | rcode |  |
| `INFCONSTRSVCE` | rcode |  |
| `CONTRACTINGSVCE` | rcode |  |
| `PASSENGERTRANS` | rcode |  |
| `AIRPASSENGER` | rcode |  |
| `PASSENGEROTHER` | rcode |  |


### Non-Energy Materials

45 - Non-Energy Materials

| Factor | Params | Variant |
|--------|--------|---------|
| `MATERIALS` | rcode |  |
| `CHEM` | rcode |  |
| `CHEMCOMMOD` | rcode |  |
| `ORGANICCHEM` | rcode |  |
| `COMMODITYCHEM` | rcode |  |
| `CHEMMIX` | rcode |  |
| `CHEMSPECIAL` | rcode |  |
| `ADDITIVES` | rcode |  |
| `ADHESIVE` | rcode |  |
| `AGROCHEM` | rcode |  |
| `SANITIZE` | rcode |  |
| `CHEMMFROTHER` | rcode |  |
| `POLYMER` | rcode |  |
| `PLASTIC` | rcode |  |
| `PLASTICOTHER` | rcode |  |
| `PLASTICMFR` | rcode |  |
| `MINING` | rcode |  |
| `METAL` | rcode |  |
| `METALPARTS` | rcode |  |
| `METALOTHER` | rcode |  |
| `METALPRIMARY` | rcode |  |
| `MINERAL` | rcode |  |
| `MIXMETALMINERAL` | rcode |  |
| `ORE` | rcode |  |
| `OREBASE` | rcode |  |
| `OREOTHER` | rcode |  |
| `PRECIOUS` | rcode |  |
| `MININGOTHER` | rcode |  |
| `OREMULTI` | rcode |  |
| `ORENONMETAL` | rcode |  |
| `MININGSTREAMING` | rcode |  |
| `GASMININGDIV` | rcode |  |
| `MATCONSTR` | rcode |  |
| `ARCHITECTCOMPONENT` | rcode |  |
| `MATCONSTRGEN` | rcode |  |
| `MATCONSTRHEAVY` | rcode |  |
| `MFRPROD` | rcode |  |
| `WOODPAPER` | rcode |  |
| `WOOD` | rcode |  |
| `WOODPAPEROTHER` | rcode |  |
| `PAPER` | rcode |  |
| `PACKAGING` | rcode |  |
| `PACKAGINGMETAL` | rcode |  |
| `PACKAGINGOTHER` | rcode |  |
| `PACKAGINGPAPER` | rcode |  |
| `PACKAGINGPLASTIC` | rcode |  |
| `MATOTHER` | rcode |  |
| `TEXTILE` | rcode |  |
| `MATDIV` | rcode |  |
| `COMPMAT` | rcode |  |


### Technology

55 - Technology

| Factor | Params | Variant |
|--------|--------|---------|
| `TECH` | rcode |  |
| `ELECTRONIC` | rcode |  |
| `COMPONENTS` | rcode |  |
| `COMPONENTINTERCONNECT` | rcode |  |
| `COMPONENTMODULE` | rcode |  |
| `COMPONENTOPTOELECTRONIC` | rcode |  |
| `COMPONENTPASSIVE` | rcode |  |
| `COMPONENTDIV` | rcode |  |
| `ELECTRONICEQUIP` | rcode |  |
| `CONTRACTELECMFR` | rcode |  |
| `ELECTRONICEQUIPDIV` | rcode |  |
| `INTERCONNECTMFR` | rcode |  |
| `SEMIMFR` | rcode |  |
| `SEMIANALOG` | rcode |  |
| `SEMIDISCRETE` | rcode |  |
| `SEMIGEN` | rcode |  |
| `SEMIMEMORY` | rcode |  |
| `SEMIPROCESSOR` | rcode |  |
| `SEMIASIC` | rcode |  |
| `SEMISPECIAL` | rcode |  |
| `ELECTRONICMFR` | rcode |  |
| `SEMIEQUIPSVCE` | rcode |  |
| `SEMIMFREQUIP` | rcode |  |
| `SEMIMFRSVCE` | rcode |  |
| `HW` | rcode |  |
| `COMMERCIALELECTRONICS` | rcode |  |
| `COMMERCEEQUIP` | rcode |  |
| `SECURITYEQUIP` | rcode |  |
| `FINELECTRONICS` | rcode |  |
| `MEDIAELECTRONICS` | rcode |  |
| `OFFICEEQUIP` | rcode |  |
| `COMMERCIALELECTRONICSMFR` | rcode |  |
| `PRINTINGELECTRONICS` | rcode |  |
| `MEASURE` | rcode |  |
| `COMMEQUIP` | rcode |  |
| `BIZCOMM` | rcode |  |
| `CABLEEQUIP` | rcode |  |
| `LANEQUIP` | rcode |  |
| `COMMEQUIPOTHER` | rcode |  |
| `SATELLITEEQUIP` | rcode |  |
| `WANEQUIP` | rcode |  |
| `WIRELESSINFEQUIP` | rcode |  |
| `WIRELESSMOBILEEQUIP` | rcode |  |
| `COMPUTER` | rcode |  |
| `PERIPHERALS` | rcode |  |
| `COMPUTERSYSTEMS` | rcode |  |
| `DATASTORAGEHW` | rcode |  |
| `COMPUTERGEN` | rcode |  |
| `HWCOMPONENTS` | rcode |  |
| `CONSUMERELECTRONICS` | rcode |  |
| `AUDIOMFR` | rcode |  |
| `AUTOELECTRONICSMFR` | rcode |  |
| `CONSUMERELECTRONICSACCESS` | rcode |  |
| `VIDEOEQUIP` | rcode |  |
| `GAMING` | rcode |  |
| `CONSUMERELECTRONICSGEN` | rcode |  |
| `PHOTO` | rcode |  |
| `VIRTUALREALITY` | rcode |  |
| `WEARABLETECH` | rcode |  |
| `TECHDISTRIB` | rcode |  |
| `HWDISTRIB` | rcode |  |
| `TECHDISTRIBOTHER` | rcode |  |
| `SOFTWDISTRIB.XX1` | rcode |  |
| `SOFTWTECH` | rcode |  |
| `INTERNET` | rcode |  |
| `CONSUMERDATA` | rcode |  |
| `INTERNETMEDIA` | rcode |  |
| `INTERNETHOSTING` | rcode |  |
| `TECHSUPPORT` | rcode |  |
| `PRODATA` | rcode |  |
| `WEBDATA` | rcode |  |
| `SOFTW` | rcode |  |
| `SOFTWDESIGN` | rcode |  |
| `SOFTWENTERPRISE` | rcode |  |
| `SOFTWGAMES` | rcode |  |
| `SOFTWHOMEOFFICE` | rcode |  |
| `SOFTWINDSPECIFIC` | rcode |  |
| `SOFTWINF` | rcode |  |
| `SOFTWGEN` | rcode |  |
| `TECHCONSULTSVCE` | rcode |  |
| `TECHCONSULTGEN` | rcode |  |
| `TECHINDSPECIFIC` | rcode |  |
| `TECHCONSULT` | rcode |  |
| `TECHCONSULTNETW` | rcode |  |
| `SOFTWDISTRIB` | rcode |  |


### Telecommunications

60 - Telecommunications

| Factor | Params | Variant |
|--------|--------|---------|
| `TELECOM` | rcode |  |
| `TELECOMSS` | rcode |  |
| `TELECOMGEN` | rcode |  |
| `TELECOMOTHER` | rcode |  |
| `TELECOMINTL` | rcode |  |
| `SATELLITESVCE` | rcode |  |
| `SATELLITEINTL` | rcode |  |
| `TELECOMUSOTHER` | rcode |  |
| `TELECOMCARRIER` | rcode |  |
| `TELECOMSOFTW` | rcode |  |
| `TELECOMSOFTWSVCE` | rcode |  |
| `SATELLITEUS` | rcode |  |
| `TELECOMAMEREXUS` | rcode |  |
| `TELECOMASIA` | rcode |  |
| `TELECOMEUROPE` | rcode |  |
| `TELECOMMIDEAST` | rcode |  |
| `TELECOMWIRE` | rcode |  |
| `WIRELESS` | rcode |  |
| `WIRELINE` | rcode |  |


### Utilities

65 - Utilities

| Factor | Params | Variant |
|--------|--------|---------|
| `UTIL` | rcode |  |
| `UTILSS` | rcode |  |
| `ENERGYUTIL` | rcode |  |
| `UTILELEC` | rcode |  |
| `GAS` | rcode |  |
| `UTILELECGAS` | rcode |  |
| `POWER.XX1` | rcode |  |
| `POWERMULTINAT` | rcode |  |
| `POWERUS` | rcode |  |
| `POWERAMEREXUS` | rcode |  |
| `POWERASIA` | rcode |  |
| `POWERINTLOTHER` | rcode |  |
| `XMSNUS` | rcode |  |
| `XMSNMULTINAT` | rcode |  |
| `WATER` | rcode |  |
| `WATERINTL` | rcode |  |
| `WATERUS` | rcode |  |
| `WATERMULTINAT` | rcode |  |


## Math

Mathematical functions, including logs, absolute values and random numbers.

### Absolute value

Evaluates to the absolute value of expr

| Factor | Params | Variant |
|--------|--------|---------|
| `Abs()` | expr |  |


### Base 10 log

Returns the base-10 log of val

| Factor | Params | Variant |
|--------|--------|---------|
| `Log10()` | val |  |


### Calculate Percent Growth

Calculates percent as 100 * ((a - b) / abs(b))

| Factor | Params | Variant |
|--------|--------|---------|
| `%()` | a , b |  |


### Constrains to a max and/or a min

Constrains a value to a maximum or a minimum. When returnNA is set to TRUE the function returns NA if expression exceeds the minimum or maximum.

| Factor | Params | Variant |
|--------|--------|---------|
| `Bound()` | expression, min, max [, returnNA] |  |
| `LBound()` | expression, min [, returnNA] |  |
| `UBound()` | expression, max [, returnNA] |  |


### Growth Rate Annualized

Calculates the annual growth rate as 100 * (pow(1 + (a - b) / abs(b), 1/years) -1). When years is 1 or unspecified, calculates growth rate as 100 * ((a - b) / abs(b)).

| Factor | Params | Variant |
|--------|--------|---------|
| `Gr%()` | a , b [, years] |  |


### Modulus Operator

Modulus operation that returns the remainder of val/modulo

| Factor | Params | Variant |
|--------|--------|---------|
| `Mod()` | val, modulo |  |


### Natural Log

Returns the natural log of val

| Factor | Params | Variant |
|--------|--------|---------|
| `LN()` | val |  |


### Negate

Changes the sign of the expression.

Ex:	Negate(5) = -5

| Factor | Params | Variant |
|--------|--------|---------|
| `Negate()` | expr |  |


### Power

Returns a number raised to a power

| Factor | Params | Variant |
|--------|--------|---------|
| `Pow()` | number , power |  |


### Random Number

Random: Returns a random number uniformly distributed between 0 and 1

| Factor | Params | Variant |
|--------|--------|---------|
| `Random` |  |  |


### Replace NA Number (Not Available)

Returns the value of expr1 if it's not NA, otherwise it returns expr2

| Factor | Params | Variant |
|--------|--------|---------|
| `IsNA()` | expr1, expr2 |  |


### Replace Negative Number

Returns the value of expr1 if it's not negative, otherwise it returns expr2

| Factor | Params | Variant |
|--------|--------|---------|
| `IsNeg()` | expr1, expr2 |  |


### Replace Negative or NA Number

Returns the value of expr1 if it's not negative and not NA, otherwise it returns expr2

| Factor | Params | Variant |
|--------|--------|---------|
| `IsNegOrNA()` | expr1, expr2 |  |


### Replace Zero Number

Returns the value of expr1 if it's not zero, otherwise it returns expr2

| Factor | Params | Variant |
|--------|--------|---------|
| `IsZero()` | expr1, expr2 |  |


### Truncate number

Rounds val toward zero

| Factor | Params | Variant |
|--------|--------|---------|
| `Trunc()` | val |  |


## Regression

Regression functions and statistics

### Linear Regression of XY Values

Operates a regression on a set of XY values.

| Factor | Params | Variant |
|--------|--------|---------|
| `LinRegXYVals()` | x0, y0, x0, y1, ..., x50, y50 |  |


### Linear Regressions of Values

Operates a regression on a set of Y values.

| Factor | Params | Variant |
|--------|--------|---------|
| `LinRegVals()` | y0, y1, ..., y50 |  |


## Regression Stats

Statistics for a previously computed regression.

### Coefficient of Determination

Returns the R² for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `R2` |  |  |


### Correlation Coefficient

Returns the R for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `R` |  |  |


### Regression Estimate

Returns the Y estimate for a previously computed XY regression.

| Factor | Params | Variant |
|--------|--------|---------|
| `EstimateXY()` | X |  |
| `EstimateY()` | offset |  |


### Regression Growth

Returns the growth for a previously computed time series regression. The period parameter can be used to annualize the growth

| Factor | Params | Variant |
|--------|--------|---------|
| `RegGr%()` | [period=1] |  |


### Regression Samples (Observations)

Returns the number of samples for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `Samples` |  |  |


### Regression Surprise

Returns the surprise of the estimated Y vs actual for a previously computed regression. Note that offset depends on the regression. Please see the Full Description

| Factor | Params | Variant |
|--------|--------|---------|
| `SurpriseY()` | offset |  |


### Slope Confidence %

Confidence is defined as 100 * (1-SlopePVal) for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `SlopeConf%` |  |  |


### Slope of the regression

Returns the Slope for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `Slope` |  |  |


### Slope p-value

Returns the P-value of the slope for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `SlopePVal` |  |  |


### Slope Standard Error

Returns the Slope Standard Error for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `SlopeSE` |  |  |


### Slope t-statistic

Returns the t Stat of the slope for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `SlopeTStat` |  |  |


### Standard Error of the Y Estimate (Sy.x)

Returns the SE of the Y estimate for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `SE` |  |  |


### Y Intercept

Returns the Y-Intercept for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `Intercept` |  |  |


### Y Intercept Standard Error

Returns the Y-Intercept Standard Error for a previously computed regression

| Factor | Params | Variant |
|--------|--------|---------|
| `InterceptSE` |  |  |


## Set

Functions that perform mathematical functions on finite data sets.

### Average of a set of values

Returns the average value in list. Up to 20 parameters are allowed and NAs are discarded

| Factor | Params | Variant |
|--------|--------|---------|
| `Avg()` | x1, x2[, .., x20] |  |


### Calculate the max/min in a set

Returns the largest value in list. Up to 20 parameters are allowed and NAs are discarded

| Factor | Params | Variant |
|--------|--------|---------|
| `Max()` | x1, x2[, .., x20] |  |
| `Min()` | x1, x2[, .., x20] |  |


### Check if an expression is in a set

Returns TRUE (1) if 'expression' is found in the list of parameters. For example, to screen for stocks in one of three industries you can write:

InSet(Industry,ADVERT,CASINO,HOTELS)

| Factor | Params | Variant |
|--------|--------|---------|
| `InSet()` | expression, x1[, ..x20]] |  |


### Count higher/lower values in a set

Returns the number of times xi > xi+1. For example to find companies that price increased at least 2 out of 3 days enter:

Higher(Close(0),Close(1),Close(2),Close(3))>=2

| Factor | Params | Variant |
|--------|--------|---------|
| `Higher()` | x1, x2[, .., x20] |  |
| `Lower()` | x1, x2[, .., x20] |  |


### Median of a set of values

Returns the median value in list. Up to 20 parameters are allowed and NAs are discarded

| Factor | Params | Variant |
|--------|--------|---------|
| `Median()` | x1, x2[, .., x20] |  |


### Standard deviation of a set of values

Returns the Relative Standard Deviation (SD divided by the mean) of the parameters.

| Factor | Params | Variant |
|--------|--------|---------|
| `RelStdDev()` | x1, x2[, .., x20] |  |
| `StdDev()` | x1, x2[, .., x20] |  |


## Utility

Functions that perform logical evaluations, provide timing information or setting variables.

### As-Of Date

Returns the current trading day as a number in the following format YYYYMMDD

| Factor | Params | Variant |
|--------|--------|---------|
| `AsOfDate` |  |  |


### Date

Returns the number of bars since the given date. Date is a number in this format YYYYMMDD.

| Factor | Params | Variant |
|--------|--------|---------|
| `BarsSince()` | date |  |
| `DaysDiff()` | from, to |  |
| `DaysSince()` | date |  |
| `PrevBarDaysAgo` |  |  |
| `Year` |  |  |
| `Month` |  |  |
| `MonthDay` |  |  |
| `WeekDay` |  |  |


### Foreign exchange rate

FXRate gives you the foreign exchange rate used to convert the currency of the stock (or ETF) to the currency in the screen/ranking system/simulation.

| Factor | Params | Variant |
|--------|--------|---------|
| `FXRate` |  |  |


### Holiday

Returns TRUE (1) if weekday is a holiday, FALSE (0) otherwise. Use negative values to check for upcoming holidays. (Note: It doesn't support checking future dates.)

| Factor | Params | Variant |
|--------|--------|---------|
| `Holiday()` | weekday | Weekday |


### Trading day in month

Returns 1 (TRUE) if the as-of date is the nth trading day of the month. Negative offsets are evaluated relative to end of month (e.g. -2 is the second-to-last trading day of the month). In multi-country regions, country code must be specified. MonthBars is intended to be used in strategies, not screens or ranking systems.

| Factor | Params | Variant |
|--------|--------|---------|
| `MonthBars()` | bars[, "cid"] |  |


### Set Variable

Sets the variable @myvar to the expression and returns TRUE. You can use the variable in subsequent rules.

| Factor | Params | Variant |
|--------|--------|---------|
| `SetVar()` | @myvar, expression |  |


### Between

Returns TRUE (1) if value is between min and max (inclusive), FALSE(0) otherwise

| Factor | Params | Variant |
|--------|--------|---------|
| `Between()` | value, min, max |  |


### Evaluate condition and return one of two values

Executes expr1 if the condition evaluates to non-zero, or expr2 otherwise. See Full Description for examples of the many uses of Eval()

| Factor | Params | Variant |
|--------|--------|---------|
| `Eval()` | condition, expr1, expr2 |  |


### GetSeries

Use this function in functions that have a 'series' parameter. You can use any stock, ETF, index ticker, or a custom series. If you use a stock ticker, your function may stop working if the ticker changes.

See Full Description for the list of index tickers and examples.

| Factor | Params | Variant |
|--------|--------|---------|
| `GetSeries()` | "ticker/series" |  |


## Constants

Identification codes of data points and series accessible across many functions.

### Dividend Date

Announce date

| Factor | Params | Variant |
|--------|--------|---------|
| `#AnnDate` | div_dt |  |
| `#ExDate` | div_dt |  |
| `#PayDate` | div_dt |  |


### Dividend Type

Any kind of dividend

| Factor | Params | Variant |
|--------|--------|---------|
| `#AllDiv` | div_type |  |
| `#Regular` | div_type |  |
| `#Special` | div_type |  |


### Formula Functions Include NA Parameter

Exclude NA values

| Factor | Params | Variant |
|--------|--------|---------|
| `#ExclNA` | incl_na |  |
| `#InclNA` | incl_na |  |
| `#NANeutral` | incl_na |  |


### Numerical Constants

Returns 62, the approximate number of bars in 3 months

| Factor | Params | Variant |
|--------|--------|---------|
| `#Month3` | period_bar | 3 Months |
| `#Month6` | period_bar | 6 Months |
| `NA` |  |  |
| `TRUE` | zeroIsNA, excl_zero, ex_zero, ex_adrs, cnt_flag |  |
| `FALSE` | zeroIsNA, excl_zero, ex_zero, ex_adrs, cnt_flag |  |
| `#Year` | period_bar | 1 Year |
| `#Year2` | period_bar | 2 Years |
| `#Month` | period_bar | 1 Month |
| `#Week` | period_bar | 1 Week |


### Streak

Increasing values streak

| Factor | Params | Variant |
|--------|--------|---------|
| `#Increasing` | streak |  |
| `#NotIncreasing` | streak |  |
| `#NotPositive` | streak |  |
| `#Positive` | streak |  |


### Actual Item (actual_item)

Capital Expenditure

| Factor | Params | Variant |
|--------|--------|---------|
| `#CAPX` | actual_item |  |
| `#EBIT` | actual_item |  |
| `#EBITDA` | actual_item |  |
| `#EPS` | actual_item |  |
| `#EPS_GAAP` | actual_item |  |
| `#FCF` | actual_item |  |
| `#FFO` | actual_item |  |
| `#NET` | actual_item |  |
| `#PTI` | actual_item |  |
| `#SALES` | actual_item |  |
| `#SHS_REPURCH` | actual_item |  |
| `#SOE` | actual_item |  |


### Consensus Estimate (cons_item)

CapEx Next Twelve Months

| Factor | Params | Variant |
|--------|--------|---------|
| `#CAPXNTM` | cons_item |  |
| `#CAPXQ` | cons_item |  |
| `#CAPXY` | cons_item |  |
| `#EBITDANTM` | cons_item |  |
| `#EBITDAQ` | cons_item |  |
| `#EBITDAY` | cons_item |  |
| `#EPSNTM` | cons_item |  |
| `#EPSQ` | cons_item |  |
| `#EPSY` | cons_item |  |
| `#FCFNTM` | cons_item |  |
| `#FCFQ` | cons_item |  |
| `#FCFY` | cons_item |  |
| `#LTG` | cons_item |  |
| `#PT` | cons_item |  |
| `#SALENTM` | cons_item |  |
| `#SALEQ` | cons_item |  |
| `#SALEY` | cons_item |  |


### Consensus Recommendation (rec_stat)

Average of all Recommendation

| Factor | Params | Variant |
|--------|--------|---------|
| `#AvgRec` | rec_stat |  |
| `#BuyCnt` | rec_stat |  |
| `#HoldCnt` | rec_stat |  |
| `#OverCnt` | rec_stat |  |
| `#RecCnt` | rec_stat |  |
| `#SellCnt` | rec_stat |  |
| `#UnderCnt` | rec_stat |  |


### Corporate Actions (ca_retvalue)

Number of actions that matched or 0

| Factor | Params | Variant |
|--------|--------|---------|
| `#ACTIONCNT` | ca_retvalue |  |
| `#ACTIONTYPE` | ca_retvalue |  |
| `#ANNCEDAYS` | ca_retvalue |  |
| `#CLOSEDAYS` | ca_retvalue |  |
| `#TRUEFALSE` | ca_retvalue |  |


### Corporate Actions (ca_status)

Approval

| Factor | Params | Variant |
|--------|--------|---------|
| `#APPROVAL` | ca_status |  |
| `#COMPLETION` | ca_status |  |
| `#MEETING` | ca_status |  |
| `#OTHER` | ca_status |  |
| `#REJECTION` | ca_status |  |
| `#STATUSANY` | ca_status |  |
| `#STATUSFAIL` | ca_status |  |
| `#STATUSNA` | ca_status |  |
| `#STATUSOK` | ca_status |  |
| `#TERMINATION` | ca_status |  |


### Corporate Actions (ca_type)

Buy Offer

| Factor | Params | Variant |
|--------|--------|---------|
| `#BUYOFF` | ca_type |  |
| `#LIQUIDATION` | ca_type |  |
| `#MANDA` | ca_type |  |
| `#MANDAEXSPIN` | ca_type |  |
| `#MERGER` | ca_type |  |
| `#MERGEREL` | ca_type |  |
| `#NEWOFFER` | ca_type |  |
| `#SPINOFF` | ca_type |  |
| `#SPLIT` | ca_type |  |


### Filing Period

Annual

| Factor | Params | Variant |
|--------|--------|---------|
| `ANN` | type |  |
| `QTR` | type |  |
| `TTM` | type |  |


### N/A during preliminaries

Fallback to previous period

| Factor | Params | Variant |
|--------|--------|---------|
| `FALLBACK` | NAHandling |  |
| `KEEPNA` | NAHandling |  |
| `ZERONA` | NAHandling |  |


### Country IDs

Albania

| Factor | Params | Variant |
|--------|--------|---------|
| `ALB` | cid | Albania |
| `DZA` | cid | Algeria |
| `AND` | cid | Andorra |
| `ATG` | cid | Antigua And Barbuda |
| `ARG` | cid | Argentina |
| `ARM` | cid | Armenia |
| `AUS` | cid | Australia |
| `AUT` | cid | Austria |
| `BHS` | cid | Bahamas |
| `BHR` | cid | Bahrain |
| `BGD` | cid | Bangladesh |
| `BRB` | cid | Barbados |
| `BLR` | cid | Belarus |
| `BEL` | cid | Belgium |
| `BLZ` | cid | Belize |
| `BMU` | cid | Bermuda |
| `BOL` | cid | Bolivia |
| `BIH` | cid | Bosnia and Herzegovina |
| `BWA` | cid | Botswana |
| `BRA` | cid | Brazil |
| `BGR` | cid | Bulgaria |
| `KHM` | cid | Cambodia |
| `CAN` | cid | Canada |
| `CYM` | cid | Cayman Islands |
| `CHL` | cid | Chile |
| `CHN` | cid | China |
| `COL` | cid | Colombia |
| `CRI` | cid | Costa Rica |
| `CIV` | cid | Cote d'Ivoire |
| `HRV` | cid | Croatia (hrvatska) |
| `CUW` | cid | Curacao |
| `CYP` | cid | Cyprus |
| `CZE` | cid | Czech Republic |
| `DNK` | cid | Denmark |
| `DOM` | cid | Dominican Republic |
| `ECU` | cid | Ecuador |
| `EGY` | cid | Egypt |
| `EST` | cid | Estonia |
| `FRO` | cid | Faroe Islands |
| `FIN` | cid | Finland |
| `FRA` | cid | France |
| `DEU` | cid | Germany |
| `GHA` | cid | Ghana |
| `GIB` | cid | Gibraltar |
| `GRC` | cid | Greece |
| `GLP` | cid | Guadeloupe |
| `GGY` | cid | Guernsey |
| `VAT` | cid | Holy See |
| `HKG` | cid | Hong Kong |
| `HUN` | cid | Hungary |
| `ISL` | cid | Iceland |
| `IND` | cid | India |
| `IDN` | cid | Indonesia |
| `IRN` | cid | Iran |
| `IRQ` | cid | Iraq |
| `IRL` | cid | Ireland |
| `IMN` | cid | Isle of Man |
| `ISR` | cid | Israel |
| `ITA` | cid | Italy |
| `JAM` | cid | Jamaica |
| `JPN` | cid | Japan |
| `JEY` | cid | Jersey |
| `JOR` | cid | Jordan |
| `KAZ` | cid | Kazakhstan |
| `KEN` | cid | Kenya |
| `KWT` | cid | Kuwait |
| `LAO` | cid | Laos |
| `LVA` | cid | Latvia |
| `LBN` | cid | Lebanon |
| `LIE` | cid | Liechtenstein |
| `LTU` | cid | Lithuania |
| `LUX` | cid | Luxembourg |
| `MKD` | cid | Macedonia |
| `MWI` | cid | Malawi |
| `MYS` | cid | Malaysia |
| `MLT` | cid | Malta |
| `MUS` | cid | Mauritius |
| `MYT` | cid | Mayotte |
| `MEX` | cid | Mexico |
| `MDA` | cid | Moldova |
| `MCO` | cid | Monaco |
| `MNG` | cid | Mongolia |
| `MNE` | cid | Montenegro |
| `MSR` | cid | Montserrat |
| `MAR` | cid | Morocco |
| `NAM` | cid | Namibia |
| `NPL` | cid | Nepal |
| `NLD` | cid | Netherlands |
| `NZL` | cid | New Zealand |
| `NGA` | cid | Nigeria |
| `NOR` | cid | Norway |
| `OMN` | cid | Oman |
| `PAK` | cid | Pakistan |
| `PAN` | cid | Panama |
| `PNG` | cid | Papua New Guinea |
| `PER` | cid | Peru |
| `PHL` | cid | Philippines |
| `POL` | cid | Poland |
| `PRT` | cid | Portugal |
| `QAT` | cid | Qatar |
| `ROU` | cid | Romania |
| `RUS` | cid | Russia |
| `RWA` | cid | Rwanda |
| `VCT` | cid | Saint Vincent and Grenadines |
| `SMR` | cid | San Marino |
| `SAU` | cid | Saudi Arabia |
| `SRB` | cid | Serbia |
| `SGP` | cid | Singapore |
| `SVK` | cid | Slovakia |
| `SVN` | cid | Slovenia |
| `ZAF` | cid | South Africa |
| `KOR` | cid | South Korea |
| `ESP` | cid | Spain |
| `LKA` | cid | Sri Lanka |
| `SPM` | cid | St. Pierre and Miquelon |
| `SJM` | cid | Svalbard and Jan Mayen |
| `SWZ` | cid | Swaziland |
| `SWE` | cid | Sweden |
| `CHE` | cid | Switzerland |
| `SYR` | cid | Syria |
| `TWN` | cid | Taiwan |
| `TZA` | cid | Tanzania United Republic Of |
| `THA` | cid | Thailand |
| `TTO` | cid | Trinidad and Tobago |
| `TUN` | cid | Tunisia |
| `TUR` | cid | Turkey |
| `TCA` | cid | Turks and Caicos Islands |
| `UGA` | cid | Uganda |
| `UKR` | cid | Ukraine |
| `ARE` | cid | United Arab Emirates |
| `GBR` | cid | United Kingdom |
| `USA` | cid | United States |
| `URY` | cid | Uruguay |
| `VEN` | cid | Venezuela |
| `VNM` | cid | Viet Nam |
| `VGB` | cid | Virgin Islands (British) |
| `VIR` | cid | Virgin Islands (u.s.) |
| `ZMB` | cid | Zambia |
| `ZWE` | cid | Zimbabwe |


### Universe IDs

All Fundamentals

| Factor | Params | Variant |
|--------|--------|---------|
| `ALLFUND` | uname |  |
| `ALLSTOCKS` | uname |  |


### Universe IDs - Major USA

Dow Jones Industrial Average

| Factor | Params | Variant |
|--------|--------|---------|
| `DJIA` | uname |  |
| `NOOTC` | uname |  |
| `Prussell1000` | uname |  |
| `Prussell2000` | uname |  |
| `Prussell3000` | uname |  |
| `SP1500` | uname |  |
| `SP500` | uname |  |


### Universe IDs - Other USA

American Depositary Receipt

| Factor | Params | Variant |
|--------|--------|---------|
| `$ADR` | uname |  |
| `LargeCap` | uname |  |
| `MasterLP` | uname |  |
| `MicroCap` | uname |  |
| `MidCap` | uname |  |
| `NASD` | uname |  |
| `NASDAQ100` | uname |  |
| `NYSE` | uname |  |
| `NYSEMKT` | uname |  |
| `OTC` | uname |  |
| `SmallCap` | uname |  |
| `SP400` | uname |  |
| `SP600` | uname |  |


### Formula Functions Sort Parameter

Sort ascending

| Factor | Params | Variant |
|--------|--------|---------|
| `#ASC` | sort |  |
| `#DESC` | sort |  |


### Formula Functions Sort Style Parameter

Neutral

| Factor | Params | Variant |
|--------|--------|---------|
| `#Neutral` | sort_style |  |
| `#Top` | sort_style |  |


### Formula Functions Scope Parameter

Operate within selected universe

| Factor | Params | Variant |
|--------|--------|---------|
| `#All` | scope |  |
| `#Industry` | scope |  |
| `#Sector` | scope |  |
| `#SubIndustry` | scope |  |
| `#SubSector` | scope |  |
| `#SP500` | scope |  |
| `#Previous` | scope |  |
| `#GroupVar` | scope |  |
| `#Family` | scope |  |
| `#AssetClass` | scope |  |
| `#Region` | scope |  |
| `#Country` | scope |  |
| `#Method` | scope |  |
| `#Style` | scope |  |
| `#Size` | scope |  |
| `#ETFSector` | scope |  |


### Aggregate Method Parameter

Average the values (default, recommended)

| Factor | Params | Variant |
|--------|--------|---------|
| `#Avg` | method |  |
| `#CapAvg` | method |  |


### Aggregate Outlier Handler Parameter

Excludes outliers from the aggregation (default)

| Factor | Params | Variant |
|--------|--------|---------|
| `#Exclude` | outlier_handl |  |
| `#Winsor` | outlier_handl |  |


## Operators

Logical and mathematical operators in common use across the site.

### Boolean operators

Expr1 And Expr2: Evaluates to 1 when both Expr1 and Expr2 are non zero.

| Factor | Params | Variant |
|--------|--------|---------|
| `And` |  |  |
| `Or` |  |  |


### Logical operators

Logical Operators:
=	Equals
!=	Not Equals

!	Negate
>	Greater
<	Less
>=	Greater or equal
<=	Less or equal

| Factor | Params | Variant |
|--------|--------|---------|
| `= != ! < > >= <=` |  |  |


### Math operators

Mathematical Operators:
+	Sum
-	Subtract
*	Multiply
/	Divide
^	Power (x^y is x raised to the power of y)

| Factor | Params | Variant |
|--------|--------|---------|
| `+ - * / ^` |  |  |


### Precedence operators

Precedence Operators:
Use parentheses to change the order operations are calculated. For example:

( 10 + 5 ) / 5 = 3
10 + 5 / 5 = 11

When in doubt, always use parentheses.

| Factor | Params | Variant |
|--------|--------|---------|
| `( )` |  |  |


### Rule comments

Allows you to add comments to a rule. Everything after // is ignored. Example:

Close(0)>5 // this is a comment

| Factor | Params | Variant |
|--------|--------|---------|
| `//` |  |  |


### Show/Set Variable operator

Following rule "@myvar:expression" sets a variable @myvar to expression, returns the expression, and displays @myvar in the screen report

| Factor | Params | Variant |
|--------|--------|---------|
| `:` |  |  |

