# Flood Risk Assessment – Rocha Department, Uruguay

## Project Overview

This project presents a GIS-based Flood Risk Assessment for Rocha Department, Uruguay, using Multi-Criteria Decision Analysis (MCDA) and raster-based spatial analysis.

The objective is to identify areas with different flood risk levels by integrating several environmental factors into a weighted flood risk model.

---

## Study Area

Rocha Department, Uruguay

---

## Objectives

- Produce a flood risk map.
- Integrate multiple environmental variables.
- Demonstrate raster analysis workflow using QGIS.
- Build a professional GIS portfolio project.

---

## Data Sources

| Dataset | Source |
|----------|--------|
| Copernicus DEM GLO-30 | Copernicus Programme |
| HydroRIVERS v1.0 | HydroSHEDS |
| ESA WorldCover 2021 | European Space Agency |

---

## Software

- QGIS 3.28
- GDAL
- GRASS GIS

---

## Methodology

The flood risk index was generated using a weighted overlay approach.

### Factors

- Distance to Rivers
- Elevation (DEM)
- Slope
- Land Cover

### Weights

| Factor | Weight |
|---------|-------:|
| Distance to Rivers | 30% |
| Slope | 30% |
| Elevation | 20% |
| Land Cover | 20% |

Each raster layer was reclassified into five suitability classes before performing the weighted overlay.

---

## Workflow

1. Clip datasets to the study area.
2. Generate hydrological network.
3. Calculate distance to rivers.
4. Reclassify river distance.
5. Generate slope from DEM.
6. Reclassify slope.
7. Reclassify elevation.
8. Reclassify land cover.
9. Align raster resolution.
10. Weighted overlay.
11. Classify flood risk.
12. Produce final cartographic layout.

---

## Outputs

- Flood Risk Index Raster
- Flood Risk Classification
- Final Cartographic Map

---

## Results

The final flood risk map classifies the study area into five categories:

- Very Low
- Low
- Moderate
- High
- Very High

---

## Skills Demonstrated

- Raster Analysis
- Hydrological Analysis
- Multi-Criteria Decision Analysis (MCDA)
- Spatial Modeling
- Terrain Analysis
- Cartographic Design
- Environmental GIS

---

## Author

**Abdallah Rafa**

GIS Analyst