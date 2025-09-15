+++
title = "Frozen-Water-Path from Arctic Weather Satellite: Level-2 Product"
date = 2025-09-10
description = "Atmospheric ice-mass retrievals from the arctic weather satellite."
[extra]
preview_image = 'aws_radiometer.jpg'
teaser_image = "teaser.png"
resources = [
    {label="Preview Dataset", link="https://storage.googleapis.com/petermfiles/cawd-aws-v0.0.1-example/html/index.html"},
    {label="Arctic Weather Satellite", link="https://www.esa.int/Applications/Observing_the_Earth/Meteorological_missions/Arctic_Weather_Satellite"},
    {label="Perforemance evaluation of AWS data", link="https://arctic-weather-satellite.org/"},
]
+++

# Description
The Chalmers Atmospheric Water Dataset from the Arctic Weather Satellite (CAWD-AWS) offers the first satellite-based estimates of atmospheric ice particle properties derived from passive microwave measurements.

This dataset is a [level 2](https://www.earthdata.nasa.gov/learn/earth-observation-data-basics/data-processing-levels) processing of the Arctic Weather Satellite (AWS) level 1B instrument data, as [provided by EUMETSAT](https://data.eumetsat.int/product/EO:EUM:DAT:0905). Thus, data is provided in the instrument's native along-track and across-track data-dimensions. The retrieval methodology builds on the work described in [May et al. (2024)](https://doi.org/10.5194/amt-17-5957-2024).

CAWD-AWS provides not only estimates but also quantiles for the following properties:
| Variable | Unit | Description |
| :-- | :-- | :-- |
| Frozen Water Path (FWP) | \\( \mathrm{kg}/\mathrm{m}^2 \\) | Mass of ice in a vertical column through the atmosphere. |
| \\(D_m\\) | \\( \\mathrm{m} \\) | Mean particle volume-equivalent-diameter in the vertical column. |
| \\(Z_m\\) | \\( \\mathrm{m} \\) | Mean particle altitude weighted by particle mass. |


Currently, only a preview subset of a few days is publicly available. We plan to continuously process and publish more soon. Sign up [here](https://forms.office.com/Pages/ResponsePage.aspx?id=ZXoUKW1T-UO4AuChtc-dvzoW4eni9cRJuq9w4XVlkQlUNEVTNlJQMUhJQ04wMUFESFBFR0c1MjFOUi4u) to be notified when more data is available.

Contact [peter.mcevoy@chalmers.se](mailto:peter.mcevoy@chalmers.se).
