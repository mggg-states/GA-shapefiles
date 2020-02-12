# Georgia Election Shapefile
This shapefile was obtained from the Georgia General Assembly Legislative and Congressional Reapportionment Office and processed by members of the Metric Geometry and Gerrymandering Group (MGGG). 

## Sources
Precinct and district shapefiles were downloaded from the [Georgia General Assembly Legislative and Congressional Reapportionment Office’s website](http://www.legis.ga.gov/Joint/reapportionment/en-US/default.aspx). Precinct level election data was obtained from the [MIT Elections Data and Science Lab](https://electionlab.mit.edu). Demographic data was downloaded from the 2010 Decennial Census at the census block level from [IPUMS NHGIS](https://www.nhgis.org).

## Processing
Election data from the MIT Elections Data and Science Lab was cleaned by MGGG staff in order to join it to the 2016 precinct shapefile. Demographic data was aggregated from the block level to the precinct level using the [assign.py script](https://github.com/maxhully/spatial-ops/tree/master/spatial_ops). Congressional, house, and senate districts were assigned to precincts using [MGGG’s roundoff code](https://github.com/gerrymandr/Preprocessing).

## Metadata
* `ID`: Unique identifier
* `DISTRICT`: County FIPS code and precinct identifier
* `PRECINCT_I`: Precinct identifier
* `PRECINCT_N`: Precinct name
* `CTYNAME`: County name
* `FIPS1`: State and county FIPS code
* `FIPS2`: County FIPS code
* `COUNTY_NAM`: County name
* `PRES16D`: Number of votes for 2016 Democratic presidential candidate
* `PRES16R`: Number of votes for 2016 Republican presidential candidate
* `PRES16L`: Number of votes for 2016 Libertarian presidential candidate
* `SEN16D`: Number of votes for 2016 Democratic senate candidate
* `SEN16R`: Number of votes for 2016 Republican senate candidate
* `SEN16L`: Number of votes for 2016 Libertarian senate candidate
* `TOTPOP`: Total population 
* `NH_WHITE`: White, non-hispanic, population
* `NH_BLACK`: Black, non-hispanic, population
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population
* `NH_ASIAN`: Asian, non-hispanic, population
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population
* `NH_OTHER`: Other race, non-hispanic, population
* `NH_2MORE`: Two or more races, non-hispanic, population
* `HISP`: Hispanic population
* `H_WHITE`: White, hispanic, population
* `H_BLACK`: Black, hispanic, population
* `H_AMIN`: American Indian and Alaska Native, hispanic, population
* `H_ASIAN`: Asian, hispanic, population
* `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population
* `H_OTHER`: Other race, hispanic, population
* `H_2MORE`: Two or more races, hispanic, population
* `VAP`: Total voting age population
* `HVAP`: Hispanic voting age population
* `WVAP`: White, non-hispanic, voting age population
* `BVAP`: Black, non-hispanic, voting age population
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population
* `ASIANVAP`: Asian, non-hispanic, voting age population
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population
* `OTHERVAP`: Other race, non-hispanic, voting age population
* `2MOREVAP`: Two or more races, non-hispanic, voting age population
* `CD`: US Congressional district
* `HDIST`: Georgia House district
* `SEND`: Georgia Senate district

## Projection
This shapefile uses EPSG: 4019.

## Rating
We give this shapefile an A rating. All data was obtained from the state government and was processed by MGGG staff.
