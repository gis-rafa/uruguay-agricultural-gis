# Land Use Change Detection Using Sentinel-2 and NDVI
### Rocha Department, Uruguay (2019–2026)

## Project Overview

This project analyzes land use and vegetation changes in Rocha Department, Uruguay, using Sentinel-2 satellite imagery and the Normalized Difference Vegetation Index (NDVI).

Google Earth Engine was used for image processing and change detection, while QGIS was used to create a professional cartographic layout.

---

## Objectives

- Detect vegetation changes between 2019 and 2026.
- Calculate NDVI for both years.
- Produce a Delta NDVI change map.
- Quantify vegetation increase, decrease, and stable areas.
- Create publication-quality maps for GIS portfolio purposes.

---

## Study Area

**Location:** Rocha Department, Uruguay

Rocha is located in southeastern Uruguay and contains agricultural land, wetlands, forests, coastal ecosystems, and protected natural areas.

---

## Software Used

- Google Earth Engine
- QGIS
- Sentinel-2 SR Harmonized
- FAO GAUL Administrative Boundaries

---

## Workflow

1. Load Rocha administrative boundary.
2. Filter Sentinel-2 imagery.
3. Create annual median composites.
4. Calculate NDVI for 2019.
5. Calculate NDVI for 2026.
6. Compute Delta NDVI.
7. Classify vegetation change.
8. Calculate area statistics.
9. Export GeoTIFF.
10. Design final map in QGIS.

---

## Results

| Category | Area (km²) | Percentage |
|-----------|-----------:|-----------:|
| Vegetation Increase | **2,597.18** | **23.41%** |
| Vegetation Decrease | **1,202.01** | **10.83%** |
| Stable Area | **7,293.86** | **65.73%** |

**Total Study Area:** **11,096.41 km²**

---

## Key Findings

- Most of Rocha remained environmentally stable during the study period.
- Vegetation gains exceeded vegetation losses.
- Approximately one quarter of the department experienced positive vegetation changes.

---

## Repository Structure

```
08-land-use-change-detection/
│
├── README.md
├── methodology.md
├── data_sources.md
├── maps/
├── outputs/
└── gee/
```

---

## Author

**Abdallah Mahmoud Farag**

GIS Analyst

Alexandria, Egypt