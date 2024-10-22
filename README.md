# Global Flood Database

If you use this database, please consider citing our work:

Li, Z., Chen, M., Gao, S., Gourley, J. J., Yang, T., Shen, X., Kolar, R., and Hong, Y.: A multi-source 120-year US flood database with a unified common format and public access, Earth Syst. Sci. Data, 13, 3755–3766, https://doi.org/10.5194/essd-13-3755-2021, 2021.


<img src="src/flowchart.png">

|ID|Sources|availabel period|accessible url|
|--|-------|----------------|--------------|
|1|Noaa Storm Database| 1950 - |https://www.ncdc.noaa.gov/stormevents/|
|2|Dartmond Flood Observatory| 1985 - |https://floodobservatory.colorado.edu/Archives/index.html|
|3|CyberFlood| 1998 - 2008| [Wan et al. (2014)](https://doi.org/10.1016/j.envsoft.2014.04.007)|
|4|Indian Flood Inventory| 1950 - ||
|5|EM-DAT (impact-based global flood archive)|1900 - |https://public.emdat.be/data|
|6|mPing|2013 - |https://mping.ou.edu/|
|7|GFM (Global Flood Monitor)|2014 - |https://www.globalfloodmonitor.org/|



|Version|create date|update|
|-------|----|------|
|IFI_1104.csv|20201104|remove invalid datetiem e.g., '!#VALUE' and convert all datetime into uniform format %Y%m or %Y%m%d|
|mPing_1030.csv|20201107|query flood data from mPing on 2020-10-30|
|cyberFlood_1104.csv|20201104|replace country code with country name; replace cause code with cause string; convert datetime to uniform format %Y%m%d|
|gfm_v0.1.csv|20201116|geocode place id to (lon,lat), and country, state|
|GFD_v0.1.csv|20201104|merged sources (1,2,3,and 4); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT','COUNTRY', 'STATE','CAUSE','AREA', 'FATALITY', 'DAMAGE', 'SEVERITY','SOURCE_DB', 'SOURCE_ID'|
|GFD_v0.2.csv|20201104|merged sources (1,2,3,4,and 5); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE','LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
|GFD_v0.21.csv|20201104|merged sources (1,2,3,4,5,and 6); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE', 'LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
|GFD_v0.22|20201107|unify country names and causes (heavy rain; snowmelt; dam break/release; ice jam; storm); filled empty country names from (lon, lat)|
|GFD_v0.30|20201116|merged sources (1,2,3,4,5,6,7), adapted from v0.22, unified country names and extracted (lon,lat) from description|
|GFD_v0.40|20201120|merged GFM based on v0.30|
|GFD_v0.42|20201123|add descriptors: distance to rivers, contributing area, flood zone, slope, DEM, LULC|
|GFD_v0.45|20201130|filter out non-numeric values in descriptors: distance to rivers, contributing area, flood zone, slope, DEM, LULC|
