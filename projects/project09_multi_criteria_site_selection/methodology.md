# Methodology

## Overview

This project applies a Multi-Criteria Decision Analysis (MCDA) approach using Google Earth Engine (GEE) to evaluate agricultural land suitability in Rocha Department, Uruguay.

Five environmental criteria were selected, standardized, weighted, and combined using a weighted overlay model.

---

# Workflow

## 1. Study Area

The administrative boundary of Rocha Department was extracted from the FAO GAUL Level-1 dataset.

---

## 2. Digital Elevation Model

Dataset:

- USGS SRTM 30 m DEM

Derived products:

- Elevation
- Slope

---

## 3. Slope Analysis

Slope was calculated from the DEM using the built-in terrain functions in Google Earth Engine.

Lower slopes received higher suitability scores because they are generally more favorable for agricultural activities.

Weight:

**30%**

---

## 4. Elevation Analysis

Elevation values were reclassified into suitability classes.

Lower elevations were assigned higher suitability scores according to the project criteria.

Weight:

**20%**

---

## 5. Distance to Rivers

HydroRIVERS was used to represent the river network.

A Euclidean distance raster was generated.

Locations closer to rivers received higher suitability scores.

Weight:

**20%**

---

## 6. Vegetation Analysis (NDVI)

Sentinel-2 imagery was used to calculate the Normalized Difference Vegetation Index (NDVI).

Higher NDVI values indicate healthier vegetation and received higher suitability scores.

Weight:

**20%**

---

## 7. Land Cover

ESA WorldCover 2021 was used to classify land cover.

Agricultural and natural vegetation classes were assigned higher suitability scores than urban areas and permanent water bodies.

Weight:

**10%**

---

# Weighted Overlay Model

The final suitability index was calculated using the following weighted equation:

Suitability =
(0.30 × Slope Score)
+ (0.20 × Elevation Score)
+ (0.20 × River Score)
+ (0.20 × NDVI Score)
+ (0.10 × Land Cover Score)

---

# Output

The final output is a continuous agricultural suitability raster with values ranging from low suitability to high suitability.

The map was exported from Google Earth Engine and finalized in QGIS for visualization and cartographic design.

---

# Software

- Google Earth Engine
- QGIS
- JavaScript

---

# Coordinate Reference System

WGS 84 / UTM Zone 21S (EPSG:32721)

---

# Final Deliverables

- Agricultural Suitability Map
- GeoTIFF Raster
- Google Earth Engine Script
- Project Documentation