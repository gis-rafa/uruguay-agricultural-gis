# Project 01 - Uruguay Base Map

## Goal

Create a clean first QGIS map of Uruguay and document the full workflow.

## Why This Project Exists

This is not meant to be impressive. It is meant to prove the foundation:

- QGIS launches and saves projects correctly.
- Layers can be loaded.
- CRS and data sources are documented.
- A simple map can be exported.

## Deliverables

- `uruguay-base-map.qgz`
- `uruguay-base-map-day-005.png`
- `uruguay-base-map-day-005.pdf`
- Data source notes
- Short project summary

## Method Notes

- Opened the Natural Earth countries layer in QGIS.
- Selected Uruguay from the world countries layer.
- Exported the selected Uruguay feature as `data/processed/uruguay_boundary.geojson`.
- Styled Uruguay with green fill and dark border.
- Confirmed project CRS: `EPSG:4326`.
- Confirmed layer CRS: `EPSG:4326`.
- Removed the original world countries layer from the active project.
- Renamed the active layer to `Uruguay Boundary`.
- Created a QGIS Print Layout titled `Uruguay Base Map`.
- Added title, author name, data source, north arrow, and scale bar.
- Exported the Day 5 layout as PNG and PDF.

## Data Source Table

| Dataset | Provider | Source / URL | Format Used | Date Accessed | Use In Project | Limitation |
|---|---|---|---|---|---|---|
| Natural Earth Admin 0 Countries | Natural Earth | https://www.naturalearthdata.com/downloads/10m-cultural-vectors/ | Shapefile, exported to GeoJSON | 2026-06-10 | Used to select and export the Uruguay national boundary | Good for a basic country boundary map, not detailed agricultural or land analysis |
## Limitations

- This is a basic boundary map only.
- It does not show departments, cities, roads, soil, elevation, or agricultural data yet.
- The data source is suitable for a first portfolio map, not detailed land analysis.
- The scale bar still needs improvement in a later layout version because the current whole-country map scale display is not ideal.

## Outputs

- `maps/uruguay-base-map-day-002.png`
- `maps/uruguay-base-map-day-003.png`
- `maps/uruguay-base-map-day-003.pdf`
- `projects/01-uruguay-base-map/uruguay-base-map-day-005.png`
- `projects/01-uruguay-base-map/uruguay-base-map-day-005.pdf`

## Next Step

Start Project 02 by collecting and documenting CONEAT / Uruguay soil-productivity data sources.
