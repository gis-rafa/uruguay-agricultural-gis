# NDVI Analysis using Sentinel-2 & QGIS
## Project Overview

This project demonstrates how to calculate the Normalized Difference Vegetation Index (NDVI) using Sentinel-2 Level-2A imagery in QGIS.

The study area is located in Rocha Department, Uruguay. The objective was to evaluate vegetation health and produce a professional GIS map suitable for a portfolio project.
Project Overview

## Objectives

- Assess vegetation health using the Normalized Difference Vegetation Index (NDVI).
- Process Sentinel-2 Level-2A imagery in QGIS.
- Produce a professional cartographic map.
- Build a portfolio-ready remote sensing project.
## Study Area

**Location:** Rocha Department, Uruguay

Rocha is located in southeastern Uruguay and is well known for its agricultural land, grasslands, wetlands, and coastal lagoons. These characteristics make it an excellent area for vegetation analysis using satellite imagery.
## Data Sources

| Dataset | Source |
|---------|--------|
| Sentinel-2 MSI Level-2A | Copernicus Data Space Ecosystem |
| Rocha Department Boundary | IDEuy (Uruguay Spatial Data Infrastructure) |
## Software

- QGIS 3.x
- Sentinel-2 MSI Level-2A

## Skills Demonstrated

- Remote Sensing
- Raster Processing
- Raster Analysis
- NDVI Calculation
- Cartographic Design
- Spatial Analysis
- Sentinel-2 Processing
## Methodology

1. Download Sentinel-2 Level-2A imagery from the Copernicus Data Space Ecosystem.
2. Extract Band 4 (Red) and Band 8 (Near Infrared).
3. Mosaic the required tiles.
4. Clip the imagery to the study area.
5. Calculate NDVI using Raster Calculator.
6. Apply NDVI symbology.
7. Design the final map layout.
8. Export the final map.
## Results

The generated NDVI map shows that most of the study area is covered by healthy vegetation, which is consistent with the agricultural and grazing activities in Rocha Department.

Water bodies and coastal lagoons appear with low or negative NDVI values, confirming that the vegetation index was calculated successfully.
## Future Improvements

- Perform multi-temporal NDVI analysis.
- Compare seasonal vegetation changes.
- Integrate NDVI with slope and soil data.
- Develop a complete land suitability model.
- Implement the workflow using Google Earth Engine.
## Project Structure

```text
04-ndvi-crop-monitoring/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── maps/
│   ├── NDVI_Rocha.png
│   └── NDVI_Rocha.pdf
│
├── qgis/
│   └── NDVI_Project.qgz
│
├── README.md
└── LICENSE
```