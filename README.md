# Global Flood Database

|ID|Sources|availabel period|accessible url|
|--|-------|----------------|--------------|
|1|Noaa Storm Database| 1950 - |https://www.ncdc.noaa.gov/stormevents/|
|2|Dartmond Flood Observatory| 1985 - |https://floodobservatory.colorado.edu/Archives/index.html|
|3|CyberFlood| 1998 - 2008| [Wan et al. (2014)](https://doi.org/10.1016/j.envsoft.2014.04.007)|
|4|Indian Flood Inventory| 1950 - ||
|5|EM-DAT (impact-based global flood archive)|1900 - |https://public.emdat.be/data|
|6|mPing|2013 - |https://mping.ou.edu/|



|Version|create date|update|
|-------|----|------|
|IFI_1104.csv|20201104|remove invalid datetiem e.g., '!#VALUE' and convert all datetime into uniform format %Y%m or %Y%m%d|
|mPing_1030.csv|20201107|query flood data from mPing on 2020-10-30|
|cyberFlood_1104.csv|20201104|replace country code with country name; replace cause code with cause string; convert datetime to uniform format %Y%m%d|
|GFD_v0.1.csv|20201104|merged sources (1,2,3,and 4); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT','COUNTRY', 'STATE','CAUSE','AREA', 'FATALITY', 'DAMAGE', 'SEVERITY','SOURCE_DB', 'SOURCE_ID'|
|GFD_v0.2.csv|20201104|merged sources (1,2,3,4,and 5); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE','LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
|GFD_v0.21.csv|20201104|merged sources (1,2,3,4,5,and 6); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE', 'LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
|GFD_v0.22|20201107|unify country names and causes (heavy rain; snowmelt; dam break/release; ice jam; storm); filled empty country names from (lon, lat)|
