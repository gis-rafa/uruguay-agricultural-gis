# Multi-Criteria Agricultural Site Suitability Analysis using Google Earth Engine

## Overview

This project presents a Multi-Criteria Decision Analysis (MCDA) workflow for identifying suitable agricultural areas in Rocha Department, Uruguay, using Google Earth Engine (GEE) and QGIS.

The analysis integrates multiple environmental factors through a weighted overlay approach to generate a final agricultural suitability map.

---

## Study Area

**Location:** Rocha Department, Uruguay

Rocha is located in southeastern Uruguay and contains diverse terrain, agricultural land, wetlands, forests, rivers, and coastal environments, making it an excellent case study for land suitability analysis.

---

## Objectives

- Identify the most suitable agricultural areas.
- Integrate multiple environmental datasets.
- Demonstrate cloud-based spatial analysis using Google Earth Engine.
- Produce a professional GIS map for decision support.

---

## Data Sources

- Google Earth Engine
- USGS SRTM 30 m DEM
- ESA WorldCover 2021
- Sentinel-2
- HydroRIVERS
- FAO GAUL 2015 Administrative Boundaries

---

## Criteria Used

| Criterion | Weight |
|-----------|-------:|
| Slope | 30% |
| Elevation | 20% |
| Distance to Rivers | 20% |
| NDVI | 20% |
| Land Cover | 10% |

---

## Workflow

1. Define the study area.
2. Import environmental datasets.
3. Generate slope from DEM.
4. Calculate distance to rivers.
5. Compute NDVI from Sentinel-2 imagery.
6. Reclassify each criterion into suitability scores.
7. Apply weighted overlay analysis.
8. Generate the final suitability map.
9. Identify optimal agricultural locations.

---

## Software

- Google Earth Engine
- QGIS
- JavaScript

---

## Results

The final output is a weighted agricultural suitability map ranging from low to high suitability across Rocha Department.

The analysis demonstrates the application of cloud GIS, remote sensing, and multi-criteria decision analysis for agricultural planning.

---

## Repository Structure

```
project09_multi_criteria_site_selection/
│
├── README.md
├── methodology.md
├── data_sources.md
├── project09_site_suitability.js
├── Project09_Rocha_Site_Suitability.png
│
└── outputs/
    ├── Rocha_Final_Suitability.tif
    └── Rocha_Best_Sites.tif
```

---

## Author

**Abdallah Rafa**

GIS Analyst | Remote Sensing

2026