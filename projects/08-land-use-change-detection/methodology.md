# Methodology

## Data Acquisition

Sentinel-2 Surface Reflectance (SR Harmonized) imagery was obtained from Google Earth Engine.

Administrative boundaries were obtained from the FAO GAUL 2015 dataset.

---

## Image Preprocessing

- Filter by Rocha boundary
- Annual image collections
- Cloud cover < 20%
- Median composite generation
- Clip to study area

---

## NDVI Calculation

NDVI was calculated using:

NDVI = (NIR − Red) / (NIR + Red)

Bands:

- B8 (Near Infrared)
- B4 (Red)

---

## Change Detection

Delta NDVI was calculated as:

Delta NDVI = NDVI2026 − NDVI2019

Interpretation:

- Positive values → Vegetation increase
- Negative values → Vegetation decrease
- Near zero → Stable vegetation

---

## Classification Thresholds

Vegetation Increase:

Delta NDVI > 0.10

Stable:

-0.10 ≤ Delta NDVI ≤ 0.10

Vegetation Decrease:

Delta NDVI < -0.10

---

## Area Calculation

Pixel area was converted into square kilometers using:

ee.Image.pixelArea()

The total area for each class was calculated using:

- Sum reducer
- 10 m spatial resolution
- Rocha administrative boundary

---

## Cartographic Design

Final maps were created in QGIS including:

- Title
- Legend
- North Arrow
- Scale Bar
- Data Sources
- Author Information