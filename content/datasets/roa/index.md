+++
title = "Rain over Africa"
date = 2023-11-05
description = "Spaceborne estimates of precipitation of Rain over Africa from geostationary (Meteosat) imagery, obtained through an artifical neural network."
[extra]
resources = [
    {label="Data", link="https://registry.opendata.aws/roa"},
    
]
preview_image = 'roa.png'
+++

# Description

## Background
Satellites are the only way to continuously monitor rainfall across all of Africa. However, current methods for estimating rain from space can take a long time because they combine data from multiple sources.

We introduced Rain over Africa (RoA) [in this publication](https://doi.org/10.1029/2025JD044595), a new public method that can provide near-real-time precipitation estimates for Africa. The approach works by downloading a [Meteosat image](https://data.eumetsat.int/data/map/EO:EUM:DAT:MSG:HRSEVIRI) and processing it with an artificial neural network trained on precipitation estimates from the calibration satellite in the Global Precipitation Measurement (GPM) mission. Note that GPM, despite being a constellation of satellites, has less continuous coverage of Africa than Meteosat.

We found that RoA estimates show good agreement with estimates from dedicated precipitation sensors. Moreover, while the latter are available every few hours at best, RoA estimates can be updated every 15 minutes. This makes RoA valuable for disaster preparedness and water management. Additionally, RoA provides practical probabilities of rain to help predict different scenarios, delivered as precipitation quantiles.

## The dataset

We are offering many years of RoA precipitation estimates via the Registry of Open Data on AWS at [registry.opendata.aws/roa](https://registry.opendata.aws/roa).

The data is stored as Zarr files in the following structure:
```
s3://rainoverafrica/
├── README.txt
└── data/
    ⋮
    ├── roa_2023.zarr/
    └── roa_2024.zarr/
```

We create one Zarr file per year and follow the pattern `roa_YYYY.zarr`. We are uploading the data in batches.

If you need to explore further the directory tree, you can use the [AWS CLI](https://github.com/aws/aws-cli) or [fsspec's s3fs](https://github.com/fsspec/s3fs).

More documentation can be found at [https://github.com/SEE-GEO/roa](https://github.com/SEE-GEO/roa).

Contact: [amell@chalmers.se](mailto:amell@chalmers.se).

## Related resources

- Amell, A., Hee, L., Pfreundschuh, S., & Eriksson, P. (2025). Probabilistic near‐real‐time retrievals of Rain over Africa using deep learning. *Journal of Geophysical Research: Atmospheres, 130*, e2025JD044595. [https://doi.org/10.1029/2025JD044595](https://doi.org/10.1029/2025JD044595)

- Rain over Africa code repository and docs: [https://github.com/SEE-GEO/roa](https://github.com/SEE-GEO/roa)

- RoA data openly accessible via the Registry of Open Data on AWS: [https://registry.opendata.aws/roa](https://registry.opendata.aws/roa)

- Rain over Africa retrievals are also available at:
    - [UK CEH Nowcasting portal](https://africa-hydrology.ceh.ac.uk/nowcasting)
    - [NCAS WISER-EWSA Catalogue](https://science.ncas.ac.uk/wiserewsa/)