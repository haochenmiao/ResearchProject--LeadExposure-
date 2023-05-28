# GIS Analysis of Cardiovascular Mortality & Estimated Lead Exposure Risk in Washington State
This project focused on understanding the geographical distribution of estimated lead exposure risk, cardiovascular mortality rates, and hospital accessibility in Washington State, with a specific focus on the southeast region.

## Overview
This project investigates how estimated lead exposure risk from housing may contribute to cardiovascular mortality rates in different census tracts of Washington (WA). Additionally, we explore how the distance from local hospitals might affect these mortality rates.

## Data
The data used in this project includes:

* Census tracts data from the Office of Financial Management.
* Estimated lead exposure risk data and cardiovascular mortality data from the Washington Tracking Network, Department of Health.
* Hospital location data within WA census tracts from the Washington Department of Health.

## Methodology
The analysis was done in QGIS and SQL. The following steps were taken:

1. Imported and visualized the census tracts data using QGIS.
2. Created a choropleth map to visualize estimated lead exposure risk from housing across WA using QGIS.
3. Generated a dot map to show the distribution of cardiovascular mortality across the state using QGIS.
4. Integrated hospital location data to explore the relationship between hospital accessibility and cardiovascular mortality. Here, SQL was used to perform a spatial join between the hospital data and the census tract data, linking each hospital to its corresponding census tract.
5. Using SQL, we performed queries on the combined dataset to select census tracts with hospitals and highlight them on the map.
6. Created a buffer to identify areas within a 3-mile radius of hospitals using QGIS.
7. Used SQL to perform queries that allowed us to identify high-risk areas, defined as those with high estimated lead exposure risk, high cardiovascular mortality, and located beyond the 3-mile radius from the nearest hospital.
8. Generated an inset map to focus on the southeast region of WA using QGIS.

## Findings
Our findings suggest a correlation between estimated lead exposure risk, cardiovascular mortality, and distance from local hospitals. The southeast region, which has the highest estimated lead exposure risk from housing, also shows a high rate of cardiovascular mortality. Many of these high-risk areas are located beyond a 3-mile radius from the nearest hospital, suggesting that distance to a hospital might exacerbate the issue.

## Limitations
While a correlation between estimated lead exposure risk, cardiovascular mortality, and distance from local hospitals was observed, the causative relationship between these variables remains unclear. Other external factors not considered in this study could also contribute to high cardiovascular mortality rates.


Here's an image of a data presentation

![Final Project](https://user-images.githubusercontent.com/83092146/227645269-54034e83-0a4b-4571-9965-e7868c2faf6a.png)
