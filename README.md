![GitHub](https://img.shields.io/badge/license-GPL--3.0-blue)

# Extract subareas and centroids from CBS postcode shapefiles

#### *Author: Marco Pellegrino, Utrecht University*

#### *April 2022 - July 2023*

## Description

This repository contains scripts to manage national CBS postcode shapefiles. Tools can extract vectorial subareas of selected postcodes and calculate their centroids. The code is generic to any subareas and it is applied to the case-study area The Hague Zuid West.

## Use

-   [PC4_centroids.R](PC4_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinates for postcodes PC4

-   [PC5_centroids.R](PC5_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinate for postcodes PC5

-   [PC6_centroids.R](PC6_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinates for postcodes PC6

-   [PC5_DHZW.R](PC5_DHZW.R) extract shapefile of PC5 postcodes for the district of The Hague Zuid West, based on the district PC4s

-   [PC6_DHZW.R](PC6_DHZW.R) extract shapefile of PC6 postcodes for the district of The Hague Zuid West, based on the district PC4s

-   [PC6_DHZW_Moerwijk.R](PC6_DHZW_Moerwijk.R) extract shapefile of PC6 postcodes where the train station Moerwijk is located. Such postcodes are used when retrieving routing information for the train trips.

## Project structure

-   root: R scripts

-   [/data](/data)

    -   [/codes](/data/codes): contains PC4 codes of the subarea, neighbourhood codes of the subarea and PC4 with the same urbanization index of the case-study subarea

    -   [/processed](/data/processed)

        -   [/csv](/data/processed/csv): csv formatted output

        -   [/shapefiles](/data/processed/shapefiles): shapefile formatted output

    -   [/raw](/data/raw): input shapefile postcode data from CBS
