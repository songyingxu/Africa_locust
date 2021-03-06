# Africa_locust
This repository contains content some scripts to calculate NDVI and surface humidity with the Google Earth Engine (GEE) in Africa area to find locust.

## Study Area
![Background](studyArea.png)
- Background Source: FAO

- Green line: study area for NDVI (25E-75E，5S-35N)

- Blue line: study area for SMAP(SSM) (25w-110E，5S-40N)

## Data source
- [MODIS_006_MOD13Q1](https://developers.google.com/earth-engine/datasets/catalog/MODIS_006_MOD13Q1)
- [SMAP](https://developers.google.com/earth-engine/datasets/catalog/NASA_USDA_HSL_SMAP_soil_moisture)
## Task 1: Soil moisture average

Calculate the soil moisture averages, soil moisture anomalies and anomaly percentages in May 2018, October 2018, and December 2019 for three months, and the 5-year historical average soil moisture for these three months.

[Open in Google Earth Engine](https://code.earthengine.google.com/7008a38d0dcfcede491be0a0ecac3b2c#workspace)


## Task 2: Monthly difference vegetation index

Vegetation index (16-day synthetic data) calculates the monthly average vegetation index to obtain the vegetation index in November 2019 (average), December 2019 (average), and January 2020 (average),  February 2020 (current value), calculate the monthly difference vegetation index (February minus January, January minus December, December minus November).

[Open in Google Earth Engine](https://code.earthengine.google.com/951dd8b59165f500d3e02208019a1a9d#workspace)

## Task 3: Half-month difference vegetation index

Vegetation index (16-day composite data), from the first period in November to the last period in February 2020, the period after November minus the previous period, and the first in December is reduced by the period after November, and the vegetation index of the second half of the month is reduced by the vegetation index of the first half of the month.

[Open in Google Earth Engine](https://code.earthengine.google.com/cf6239e87c7d83a71855267e9d2d427a#workspace)

## Task 4: Change trend graph

Vegetation index (16-day synthetic data). From the first period in November 2019 to the last period in February 2020, the linear trend of vegetation index is calculated on a pixel-by-pixel basis. The linear trend data (that is, the slope of the curve).

[Open in Google Earth Engine](https://code.earthengine.google.com/4654e8c8fd577588dfab1b4a626d5bb9#workspace)

## Task 5: Soil moisture calculation
Data is SMAP 0.25 * 0.25 degree data, calculate the average monthly soil moisture in the study area from 2018.01 to 2020.01, the monthly soil moisture anomaly value and the anomaly percentage (the average value of the anomaly is calculated from January 2015 to December 2019, each month 5 year average).

[Open in Google Earth Engine](https://code.earthengine.google.com/671d54f403b26d8b7f11daae3b19aaab#workspace)


