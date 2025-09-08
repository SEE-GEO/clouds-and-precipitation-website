+++
title = "Frozen-Water-Path from Arctic Weather Satellite: Level-2 Product"
date = 2024-01-10
description = "Atmospheric ice-mass retrievals from the arctic weather satellite."
[extra]
authors = [
    {name="Peter McEvoy", link="https://www.chalmers.se/en/persons/evoy"},
    {name="Eleanor May", link="https://www.chalmers.se/en/persons/maye/"},
    {name="Patrick Eriksson", link="https://www.chalmers.se/en/persons/patrick2/"},
]
preview_image = 'aws_radiometer.jpg'
teaser_image = "teaser.png"
resources = [
    {label="Preview Dataset", link="https://storage.googleapis.com/petermfiles/cawd-aws-v0.0.1-example/html/index.html"},
    {label="Arctic Weather Satellite", link="https://arctic-weather-satellite.org/"},
]
+++

# Description
The Chalmers Atmospheric Water Dataset from the Arctic Weather Satellite (CAWD-AWS) offers the first satellite-based estimates of atmospheric ice particle properties derived from passive microwave measurements.

This dataset represents a [level 2](https://www.earthdata.nasa.gov/learn/earth-observation-data-basics/data-processing-levels) processing of the Arctic Weather Satellite (AWS) level 1B instrument data, as [provided by EUMETSAT](https://data.eumetsat.int/product/EO:EUM:DAT:0905). Thus, data is provided in the instrument's native scan and mirror angle dimensions across the satellite's polar orbit. The retrieval methodology builds on the work described in [May et al. (2024)](https://doi.org/10.5194/amt-17-5957-2024).

CAWD-AWS provides not only estimates but also quantiles for the following properties:
| Variable | Unit | Description |
| :-- | :-- | :-- |
| Frozen Water Path (FWP) | \\( \mathrm{kg}/\mathrm{m}^2 \\) | Mass of ice in a vertical column through the atmosphere. |
| \\(D_m\\) | \\( \\mathrm{m} \\) | Mean particle volume-equivalent-diameter in the vertical column. |
| \\(Z_m\\) | \\( \\mathrm{m} \\) | Mean particle altitude weighted by particle mass. |


Currently, only a preview subset is publicly available. We plan to continuously process and publish more soon.
