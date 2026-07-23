# Data Sources

This project integrates multiple open geospatial datasets through Google Earth Engine to perform Multi-Criteria Agricultural Site Suitability Analysis for Rocha Department, Uruguay.

---

# 1. Administrative Boundaries

**Dataset**

FAO GAUL 2015 Level 1

**Purpose**

Defines the study area (Rocha Department).

---

# 2. Digital Elevation Model (DEM)

**Dataset**

USGS SRTM GL1 30 m

**Resolution**

30 meters

**Purpose**

- Elevation analysis
- Slope calculation

---

# 3. River Network

**Dataset**

HydroRIVERS v10

**Provider**

HydroSHEDS

**Purpose**

Distance-to-river analysis.

---

# 4. Satellite Imagery

**Dataset**

Copernicus Sentinel-2 SR Harmonized

**Spatial Resolution**

10 meters

**Purpose**

NDVI calculation.

---

# 5. Land Cover

**Dataset**

ESA WorldCover 2021

**Spatial Resolution**

10 meters

**Purpose**

Land cover suitability assessment.

---

# Processing Platform

- Google Earth Engine

---

# Desktop GIS

- QGIS 3.x

---

# Coordinate Reference System

WGS 84 / UTM Zone 21S

EPSG:32721

---

# Summary of Datasets

| Dataset | Purpose |
|---------|---------|
| FAO GAUL 2015 | Administrative Boundary |
| USGS SRTM DEM | Elevation & Slope |
| HydroRIVERS | Distance to Rivers |
| Sentinel-2 SR Harmonized | NDVI |
| ESA WorldCover 2021 | Land Cover |

---

# Notes

All datasets are publicly available and were accessed through the Google Earth Engine Data Catalog, except HydroRIVERS, which was uploaded as a Google Earth Engine Asset.