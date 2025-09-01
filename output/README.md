# Outputs

## Spatially Explicit Emission Maps

### General Info
 - Cells are in kg
 - Spatial resolution is 1/600° x 1/1200° (about 100m x 100m)
 - Coordinate Reference System is EPSG 25832
 - CH4 emissions are extracted from downscaled TNO inventory and not based on bottom-up calculation
 - Sectors beside A, C (includes B), F, Human Respiration are sourced from the downscaled european inventory (TNO-GHGco V4.1)
  
### GNFR A
- Some values of 2024 are not available yet and were estimated based on previous years.
### GNFR C
- Includes industry (GNFR_B) related gas/oil consumption for heating and production emissions extracted from individual EMAS reports
### GNFR F
- No additional info
### Human Respiration
- Same for all years
- Includes columns for "CO2_residential," "CO2_nonresidential," and "CO2_outdoor."

## Temporal Emission Profiles

### General Info
 - CSV files are separated by commas
 - Columns are year, component, timestamp, scaling_factor
 - Timestamps indicate time zone. Either UTC or local time (CET/CEST)
 - Wherever timezone info is missing UTC is assumed
 - Timestamps are at the start of the hour (0:00-01:00) is given as 0:00
 - Multiple profiles for different components (i.e. CO2, NOx, CO) for the same year might be concated into one file
 - Scaling factors are given for each hour of the year
 - To calculate hourly emissions the average emission (yearly CO2 / hours of corresponding year) * scaling_factor has to be calculated

  
### GNFR A
- There are additional high-resolution "internal-only" profiles for all point sources available in the NAS
### GNFR C
- No additional info
### GNFR F
- No additional info
### Human Respiration
- Profiles are available for three sub-sectors: "indoor residential," "indoor non-residential," and "outdoor."

### Other Sectors
Please refer to [Denier van der Gon et al., 2011](https://atmosphere.copernicus.eu/sites/default/files/2019-07/MACC_TNO_del_1_3_v2.pdf) for temporal profiles of other sectors.