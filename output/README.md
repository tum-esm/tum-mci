# Outputs

## Spatially Explicit Emission Maps

### General Info
 - Cells are in kg
 - Spatial resolution is 100m x 100m
 - Coordinate Reference System is EPSG 25832
 - CH4 emissions are extracted from downscaled TNO inventory and not based on bottom-up calculation
 - Sectors beside A,C (includes B),F, Human Respiration are sources from the downscaled TNO inventory
  
### GNFR A
- Some values of 2024 are not available yet and were estimated based on previous years.
### GNFR C
- Includes industry related gas/oil consumption for heating and production emissions extracted from EMAS reports
### GNFR F
### Human Respiration
- Same for all years

## Temporal Emission Profiles

### General Info
 - CSV files are separated by commas
 - Columns are year,component,timestamp,scaling_factor
 - Multiple profiles for different components might be concated in the file
 - Scaling factor is given for each hour of the year
 - To calculate hourly emissions the average emission (total year / hours of year) * hourly emissions factor has to be calculated
 - Timestamps indicate time zone. Either UTC or local time (CET/CEST)
 - Timestamps are at the start of the hour (0:00-01:00) is given as 0:00
  
### GNFR A
- There are additional high-resolution "internal-only" profiles available in the NAS
### GNFR C
### GNFR F
### Human Respiration