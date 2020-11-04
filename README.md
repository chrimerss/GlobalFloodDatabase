# Global Flood Database

|Sources|availabel period|accessible url|
|-------|----------------|--------------|
|1. Noaa Storm Database| 1950 - ||
|2. Dartmond Flood Observatory| 1985 - ||
|3. CyberFlood| 1998 - 2008||
|4. Indian Flood Inventory| 1950 - ||



|Version|create date|update|
|-------|----|------|
|IFI_1104.csv|20201104|remove invalid datetiem e.g., '!#VALUE' and convert all datetime into uniform format %Y%m or %Y%m%d|
|cyberFlood_1104.csv|20201104|replace country code with country name; replace cause code with cause string; convert datetime to uniform format %Y%m%d|
|merged_v0.1.csv|20201104|merged sources (1,2,3,and 4); formated date to be the same; headers:'DATE_BEGIN', 'DATE_END', 'DURATION', 'LON', 'LAT','COUNTRY', 'STATE','CAUSE','AREA', 'FATALITY', 'DAMAGE', 'SEVERITY','SOURCE_DB', 'SOURCE_ID'|
