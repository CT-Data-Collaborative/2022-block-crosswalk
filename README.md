# 2022 Census Block Crosswalk

#### Census block crosswalk to census tract, town, county, county equivalent, ZCTA/ZIP code, and PUMA (2020)

The 2022blockcrosswalk.csv file contains a crosswalk between 49,861 Connecticut census blocks and tracts, towns, counties, country equivalents, ZIP codes, and 2020 PUMAS in CT. 

#### Note about FIPS Codes and County Equivalents
In 2022, the Census Bureau adopted county equivalents- Connecticut's nine planning regions- as new county-level geographies for Connecticut for statistical purposes, replacing Connecticut's eight counties in Census Bureau data products. The county equivalents have new FIPS codes.

Census Bureau data and publications will transition to using the county equivalents instead of counties throughout 2023-2024. To help ease this transition, this crosswalk includes FIPS codes for both the counties and the new county equivalents.

Blocks, tracts, and towns therefore have two FIPS identifiers. The tract and town boundaries did not change.
- block_fips_20, tract_fips_20, and town_fips_20 include the FIPS code from its county (county_fips_20)
- block_fips_22, tract_fips_22, and town_fips_22 include the FIPS code from its county equivalent/planning region (ce_fips_22)

#### To prevent Excel from transforming FIPS codes and zip codes to numbers automatically (which leads to missing leading 0s), do the following:
1. Open Excel, New workbook
2. Go to File > Import > CSV file
3. Choose file, and select "text" as type of block_fips_2020, block_fips_2022, tract_fips_2020, tract_fips_2022, town_fips_2020, town_fips_2022, county_fips_2020, ce_fips_2022 and zipcode columns.

Note that blocks that contained only water and were not within municipal boundaries are excluded from this crosswalk. The blocks are in 2020 tracts 09001990000, 09007990100, 09009990000, and 09011990100.

#### Sources
- 2020 TIGER/Line Shapefiles: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2020.html
- 2022 TIGER/Line Shapefiles: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2022.html
- County subdivisions (which are towns for Connecticut) on TIGER: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2019&layergroup=County+Subdivisions
- Connecticut zipcode boundaries: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=ZIP+Code+Tabulation+Areas
