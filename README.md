# general-election-2024
 The Centre for Cities constituency data tool provides local economic data for every parliamentary constituency in Great Britain. This repo contains the master sheet for the tool.
 
## Description 

The Centre for Cities constituency data tool combines combines different datasets to the new constituency map for the 2024 general election. This tool is available here: https://www.centreforcities.org/data/constituency-data-tool/

Much of this data is not currently available at the constituency level, so Centre for Cities has used data at small geographies (LSOAs) and assigned it to the new constituencies where they overlap.

This repo contains the final mastersheet produced for this tool for every constituency in Great Britain as a CSV, plus some additional data on housing affordability and tenure. The full workbook is available on request.

## Understanding the Data

There are 26 different indicators in this dataset, including:

* Gross Income (2018), Admin-based income statistics, England and Wales: tax year ending 2018 https://www.ons.gov.uk/peoplepopulationandcommunity/personalandhouseholdfinances/incomeandwealth/articles/adminbasedincomestatisticsenglandandwales/taxyearending2018

* Commuting data (2011), Census 2011 https://www.nomisweb.co.uk/query/select/getdatasetbytheme.asp?theme=75

* Deprivation (2019), IMD by LSOA, https://opendatacommunities.org/resource?uri=http%3A%2F%2Fopendatacommunities.org%2Fdata%2Fsocietal-wellbeing%2Fimd2019%2Findices

* Qualifications (2021), Census 2021, https://www.nomisweb.co.uk/query/select/getdatasetbytheme.asp?theme=93

* Health (2021), Census 2021, https://www.nomisweb.co.uk/query/select/getdatasetbytheme.asp?theme=93

* Jobs (2022), BRES 2022, https://www.nomisweb.co.uk/query/select/getdatasetbytheme.asp?theme=27

* House Prices (2018, 2022), Land Registry Price Paid data, https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads

* Housing tenure (2021), Census 2021, https://www.nomisweb.co.uk/query/select/getdatasetbytheme.asp?theme=93

## Method

Constituencies have been classified as either urban (conforming with the Centre for Cities 2015 Primary Urban Area [PUA] boundaries, built out of local authorities with a daytime [workplace] population greater than 135,000); hinterland (within commutable distance of each PUA, varying across the country) and more rural (outside of commuting distance of a PUA) according to their LSOAs. 

LSOAs have been allocated to the seat in which a majority of their area lies. 

Each indicator is constructed from the LSOAs assigned to each constituency, with the LSOA values used as both the numerator and the denominator for each constiuency. For example, if there are 25000 people with poor health in the LSOAs that make up a constituency, and the total population of those LSOAs is recorded as 70000, then 36% of the population will be recorded as being in poor health in the constituency. This is effectively a weighted average for each seat.

## Acknowledgements

Paul Swinney for conducting the original analysis, Viola Pititto for building the original tool
