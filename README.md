![GitHub](https://img.shields.io/badge/license-GPL--3.0-blue)

## Extracting subareas and centroids from CBS postcode shapefiles

**Utrecht University, The Netherlands. 2022 - 2023**

Author: Marco Pellegrino

Contributors: Jan de Mooij, Tabea Sonnenschein, Mehdi Dastani, Dick Ettema, Brian Logan, Judith A. Verstegen

## Description

This repository contains scripts to manage national CBS postcode shapefiles. Tools can extract vectorial subareas of selected postcodes and calculate their centroids. The code is generic for any subareas and it is applied to the case-study area of the district of Den Haag Zuid-West (DHZW).

## Data Sources

Vectorial shapefiles can be retrieved from the [CBS portal](https://www.cbs.nl/nl-nl/dossier/nederland-regionaal/geografische-data/gegevens-per-postcode).

## Usage

[PC4\_centroids.R](PC4_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinates for postcodes PC4

[PC5\_centroids.R](PC5_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinate for postcodes PC5

[PC6\_centroids.R](PC6_centroids.R) extract centroids as a shapefile and CSV dataframe of coordinates for postcodes PC6

[PC5\_DHZW.R](PC5_DHZW.R) extract the shapefile of PC5 postcodes for the district of The Hague Zuid West, based on the district PC4s

[PC6\_DHZW.R](PC6_DHZW.R) extract the shapefile of PC6 postcodes for the district of The Hague Zuid West, based on the district PC4s

[PC6\_DHZW\_Moerwijk.R](PC6_DHZW_Moerwijk.R) extract the shapefile of PC6 postcodes where the train station Moerwijk is located. Such postcodes are used when retrieving routing information for train trips.

## Project structure

root: R scripts

[/data](/data)

[/codes](/data/codes): includes PC4 codes of the subarea, neighbourhood codes of the subarea and PC4 with the same urbanization index as the case-study subarea

/processed

/csv: CSV formatted output

/shapefiles: shapefile formatted output

/raw: input shapefile postcode data from CBS