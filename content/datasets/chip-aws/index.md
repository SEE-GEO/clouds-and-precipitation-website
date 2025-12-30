+++
title = "CHIP-AWS: Chalmers Hydrometeor Inversion Product from the Arctic Weather Satellite"
date = 2025-09-10
description = "Atmospheric ice-mass retrievals from the arctic weather satellite's sub-millimetre radiometer measurements."
[extra]
preview_image = 'aws_radiometer.jpg'
teaser_image = "teaser.png"
resources = [
    {label="chip-aws-v0.6", link="http://data.clouds-and-precip.group/chip-aws/chip-aws-v0.6/html/"},
]
+++

# Description
The Chalmers Hydrometeor Inversion Product from the Arctic Weather Satellite (CHIP-AWS) provides
estimates of ice hydrometeor masses in the atmosphere across the globe within the +/-60° latitude region.
The retrieval methodology is based on the work described in [May et al. (2024)](https://doi.org/10.5194/amt-17-5957-2024).

This dataset represents a [level 2](https://www.earthdata.nasa.gov/learn/earth-observation-data-basics/data-processing-levels) processing of the Arctic Weather Satellite (AWS) level 1B instrument data, as [provided by EUMETSAT](https://data.eumetsat.int/product/EO:EUM:DAT:0905). This processing level produces single-footprint retrievals with relatively high resolution (~10 km in nadir) for this type of instrument.

The following quantities are retrieved:
| Variable | Unit | Description |
| :-- | :-- | :-- |
| Frozen Water Path (FWP) | \\( \mathrm{kg}/\mathrm{m}^2 \\) | Mass of ice hydrometeors in a vertical column through the atmosphere. |
| \\(D_m\\) | \\( \\mathrm{m} \\) | Mass-weighted mean volume equivalent diameter of ice hydrometeors inside the column. |
| \\(Z_m\\) | \\( \\mathrm{m} \\) | Mass-weighted mean altitude of ice hydrometeors inside the column. |

Besides best estimates, the uncertainty is described by providing quantiles of the retrieved CDF for each variable.


The dataset is updated roughly every month with new data and is made publicly available here: <http://data.clouds-and-precip.group/chip-aws/chip-aws-v0.6/html/>.  
Sign up [here](https://forms.office.com/Pages/ResponsePage.aspx?id=ZXoUKW1T-UO4AuChtc-dvzoW4eni9cRJuq9w4XVlkQlUNEVTNlJQMUhJQ04wMUFESFBFR0c1MjFOUi4u) to be notified about significant updates
# About the Arctic Weather Satellite
More information on the satellite and its instrument can be found here:
- [ESA page on the Arctic Weather Satellite](https://www.esa.int/Applications/Observing_the_Earth/Meteorological_missions/Arctic_Weather_Satellite)
- [The Arctic Weather Satellite radiometer (2025)](https://doi.org/10.5194/amt-18-4709-2025)
- [Performance evaluation of AWS data](https://arctic-weather-satellite.org/)

Contact [peter.mcevoy@chalmers.se](mailto:peter.mcevoy@chalmers.se).
