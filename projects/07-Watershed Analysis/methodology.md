# Methodology

## Step 1 — DEM Preparation

The Copernicus DEM (30 m) was clipped to the Rocha Department boundary.

---

## Step 2 — Sink Filling

Depressions were removed from the DEM using GRASS GIS to create a hydrologically correct elevation model.

Output:

- dem_breached.tif

---

## Step 3 — Flow Direction

Flow direction was calculated using GRASS GIS.

Output:

- drainage_direction_grass.tif

---

## Step 4 — Flow Accumulation

Flow accumulation was generated from the corrected DEM.

Output:

- flow_accumulation_grass.tif

---

## Step 5 — Stream Extraction

A stream threshold was applied to extract the drainage network.

Output:

- stream_segments_thin.tif

- stream_network_rocha.gpkg

---

## Step 6 — Stream Ordering

The extracted network was classified using the Strahler stream ordering method.

Output:

- strahler_order_rocha.tif

---

## Step 7 — Cartographic Layout

A final map was designed in the QGIS Layout Manager including:

- Title
- North Arrow
- Scale Bar
- Data Source
- Author