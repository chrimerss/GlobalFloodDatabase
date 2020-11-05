# Global Flood Database

|Sources|availabel period|accessible url|
|-------|----------------|--------------|
|1. Noaa Storm Database| 1950 - ||
|2. Dartmond Flood Observatory| 1985 - ||
|3. CyberFlood| 1998 - 2008||
|4. Indian Flood Inventory| 1950 - ||
|5. EM-DAT (impact-based global flood archive)|1900 - ||
|6. mPing|2013 - |https://mping.ou.edu/|



|Version|create date|update|
|-------|----|------|
|IFI_1104.csv|20201104|remove invalid datetiem e.g., '!#VALUE' and convert all datetime into uniform format %Y%m or %Y%m%d|
|cyberFlood_1104.csv|20201104|replace country code with country name; replace cause code with cause string; convert datetime to uniform format %Y%m%d|
|merged_v0.1.csv|20201104|merged sources (1,2,3,and 4); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT','COUNTRY', 'STATE','CAUSE','AREA', 'FATALITY', 'DAMAGE', 'SEVERITY','SOURCE_DB', 'SOURCE_ID'|
|merged_v0.2.csv|20201104|merged sources (1,2,3,4,and 5); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE','LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
|merged_v0.21.csv|20201104|merged sources (1,2,3,4,5,and 6); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT', 'COUNTRY', 'STATE', 'LOCATION', 'AREA', 'FATALITY', 'DAMAGE', 'SEVERITY', 'SOURCE', 'CAUSE', 'SOURCE_DB', 'SOURCE_ID', 'DESCRIPTION'|
