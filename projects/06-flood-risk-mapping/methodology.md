# Methodology

## Overview

The flood risk assessment was developed using raster-based spatial analysis within QGIS.

The workflow combines terrain analysis, hydrological processing, land cover classification, and weighted overlay analysis.

---

# Step 1

Study Area Preparation

- Rocha Department boundary
- Coordinate System:
  - WGS 84 / UTM Zone 21S
  - EPSG:32721

---

# Step 2

Elevation Processing

Input

- Copernicus DEM GLO-30

Process

- Clip DEM
- Generate Slope

Outputs

- DEM
- Slope Raster

---

# Step 3

Hydrological Analysis

Input

HydroRIVERS

Process

- Clip river network
- Rasterize rivers
- Generate proximity raster

Output

River Distance Raster

---

# Step 4

Land Cover Processing

Input

ESA WorldCover 2021

Process

- Clip
- Reclassify

Output

Land Cover Suitability Raster

---

# Step 5

Raster Reclassification

Each dataset was reclassified into five flood susceptibility classes.

Class Values

1 = Very Low

2 = Low

3 = Moderate

4 = High

5 = Very High

---

# Step 6

Weighted Overlay

Flood Risk Index

Flood Risk =
0.30 × River Distance +
0.30 × Slope +
0.20 × Elevation +
0.20 × Land Cover

---

# Step 7

Flood Risk Classification

The flood risk index was classified into five categories.

- Very Low
- Low
- Moderate
- High
- Very High

---

# Step 8

Cartographic Design

The final layout includes

- Title
- Legend
- North Arrow
- Scale Bar
- CRS
- Data Sources
- Author

---

## Final Output

Flood Risk Assessment Map

Rocha Department

Uruguay