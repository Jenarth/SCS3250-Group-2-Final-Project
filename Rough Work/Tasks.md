# Tasks/Ideas
LW: Select 4? different weeks (months?). Needs to overlap with transit data and have no NaNs.
- Heaviest rain
- Heaviest snow
- Coldest
- Hottest
- Standard/Normal

MS: Weather Data:
- Remove unnecessary columns. (Choose relevant columns.)
- Remove rows outside of transit data range.
- Replace NaNs (nulls).
- Change Flags to boolean.
- Merge the two DataFrames.
- Plot daily ridership with daily weather

BY: 
- Correlation (boardings vs temp/precip).
- Removing outliers
  - Identify weekends and holidays (potentially as a column)

JJ: 
- Aggregate hourly transit data. Need daily totals.
- Get mean monthly temperature 
- Get the delta between daily temperature and mean monthly temperature
- Plot the delta in relation to the daily total
- Change ridership to int

VN: Add station data
- Load, clean, merge into boardings.
- Investigate prediction


Final Dataset:
- DateTime as index/rows
- Columns:
  - GO Station Name - VN 
  - GO Line Name - VN 
  - Daily Total Ridership - VN
  - Daily Mean Temp - MS
  - Daily Min Temp - MS 
  - Daily Max Temp - MS 
  - Monthly Mean Temp - JJ
  - Delta between Daily Mean Temp and Monthly Mean Temp - JJ
  - Daily Precipitation - MS
  - Monthly Precipitation (mean of daily precipitation) - JJ
  - Snow on Ground - MS
  - Day
  - Weekday
  - Month
  - Year
  - Column per GO line (aggregate daily ridership)
  - Total GO ridership
  
Ideas for data:
- Good/Bad Weather Days
  - Ex. Good/ Bad temp (releative to monthly mean temp) + precipitation

Report:
- VN writing about GO data
- MS writing about Weather data
- BY writing about correlation
