# Project 07 – Watershed Analysis of Rocha Department, Uruguay

## Overview

This project focuses on watershed analysis and stream network extraction for Rocha Department, Uruguay, using a Copernicus DEM (30 m) and GRASS GIS tools integrated within QGIS.

The workflow demonstrates a complete hydrological preprocessing chain, including DEM conditioning, flow direction, flow accumulation, stream extraction, and Strahler stream order generation.

---

## Objectives

- Prepare the DEM for hydrological analysis.
- Generate flow direction and flow accumulation rasters.
- Extract the stream network.
- Classify streams using the Strahler ordering system.
- Produce publication-quality cartographic outputs.

---

## Software

- QGIS 3.44
- GRASS GIS

---

## Data

- Copernicus DEM (30 m)
- Study Area: Rocha Department, Uruguay

---

## Outputs

- DEM after sink filling
- Flow Direction
- Flow Accumulation
- Stream Segments
- Stream Network
- Strahler Stream Order
- Final Map (PNG & PDF)

---

## Repository Structure

```
07-Watershed-Analysis/
│
├── Stream_Order_Rocha.pdf
├── Stream_Order_Rocha.png
├── dem_rocha_clipped.tif
├── dem_breached.tif
├── drainage_direction_grass.tif
├── flow_accumulation_grass.tif
├── stream_segments_thin.tif
├── strahler_order_rocha.tif
├── stream_network_rocha.gpkg
├── methodology.md
├── data_sources.md
└── README.md
```

---

Prepared by

**Abdallah Rafa**

Alexandria University

GIS Portfolio 2026