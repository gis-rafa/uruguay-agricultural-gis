# Project 02 - CONEAT Soil Productivity Mapping

## Goal

Create a first Uruguay soil-productivity map using CONEAT data and explain what the map can and cannot say.

## Main Question

How can Uruguay's CONEAT soil-productivity data be mapped in QGIS to support a basic agricultural land assessment?

## Why CONEAT Matters

CONEAT is important for Uruguay-focused agricultural GIS because it connects soil groups, land productivity, and agricultural land evaluation. This project will move the portfolio from a simple national boundary map toward soil and land-suitability analysis.

## Expected Data Sources

| Dataset | Provider | Expected Use | Status |
|---|---|---|---|
| CONEAT soil/productivity data | MGAP / Uruguay official ArcGIS REST source | Soil-productivity mapping | Loaded in QGIS |
| Uruguay boundary | Natural Earth / existing Project 01 output | National reference boundary | Available |
| Department or study-area boundary | Uruguay official source if available | Clip the CONEAT layer to a smaller area | To collect |

## Data Source Record

```text
Source name: Grupos CONEAT (1:40.000)
Provider: MGAP / Uruguay official ArcGIS REST service
URL: https://mapas.mgap.gub.uy/arcgis/rest/services/SNIA_Temas/Suelos/MapServer
Format: ArcGIS REST feature layer loaded in QGIS
Date accessed: 2026-06-23
Feature count: 33,557
Important fields: SC, OBJECTID, Shape.STArea(), Shape.STLength()
Example SC values: 07.1, 07.2, 2.21, 3.15, 3.12
Can it be loaded in QGIS? yes
```

## Work Completed

- Created an ArcGIS REST connection named `MGAP Suelos`.
- Loaded the feature layer `Grupos CONEAT (1:40.000)`.
- Confirmed the attribute table opens.
- Confirmed feature count: `33,557`.
- Identified `SC` as the main visible soil group/code field.
- Renamed the layer in QGIS to `CONEAT Soil Groups`.
- Styled the CONEAT layer with categorized symbology using the `SC` field.
- Created a first QGIS layout titled `Uruguay CONEAT Soil Groups`.
- Added title, source text, north arrow, and scale bar.
- Exported first PNG and PDF previews.
- Created a zoomed sample-area layout titled `CONEAT Soil Groups - Sample Area`.
- Exported sample-area PNG and PDF previews for improved readability.
- Wrote a first interpretation note explaining what the map shows and what it cannot prove yet.
- Created a filtered highlight layer for `SC = 07.1`.
- Made the Uruguay boundary transparent so the filtered CONEAT group is visible.
- Exported a smaller, clearer highlight map for CONEAT group `07.1`.

## Expected Map Output

- `coneat-soil-groups-day-007.png`
- `coneat-soil-groups-day-007.pdf`
- `coneat-sample-area-day-008.png`
- `coneat-sample-area-day-008.pdf`
- `coneat-group-07-1-highlight-day-009.png`
- `coneat-group-07-1-highlight-day-009.pdf`
- Data source table and limitations.

## Main Limitation

This project will be a learning and portfolio map, not a legal or agronomic recommendation. Any land-quality interpretation must be cautious and based on documented data fields, assumptions, and limitations.

The PDF exports are large because the CONEAT layer contains many detailed polygons. A later version should clip to a smaller official study area or optimize export settings.

## Interpretation Note

## Interpretation - CONEAT Group SC = 07.1

This map highlights areas classified as CONEAT group SC = 07.1 within Uruguay.

The purpose of this map is to isolate one soil/productivity group from the official CONEAT dataset and show where it appears spatially. This helps turn the raw attribute table into a clearer geographic view that can be used for agricultural GIS interpretation.

At this stage, the map should be treated as a descriptive GIS output, not as a land suitability recommendation. The official CONEAT group description now provides a basic agricultural context for group 07.1, but field validation and additional land-use data are still needed before making practical agricultural recommendations.

Data source: official MGAP / CONEAT data.

Limitations:
- The map only highlights one CONEAT group.
- The interpretation is based on the official group description, not field validation.
- The map does not include parcel-level ownership, current land use, or recent land-cover change.
- The output should not be used as a land investment or agricultural recommendation.
- Further analysis would need field data, recent imagery, and additional soil/land-use layers.
## Official CONEAT Context

According to Uruguay’s Ministry of Livestock, Agriculture and Fisheries (MGAP), CONEAT groups are used to describe homogeneous land areas based on productive capacity. They are not strictly basic soil cartographic units. The CONEAT Productivity Index expresses each group’s productive capacity relative to the national average, where the national average is 100.

For each CONEAT group, official documentation may include characteristics such as relief, parent material, soil composition, land use, and other relevant attributes.

## Specific CONEAT Group Meaning - 07.1

According to the official CONEAT group description, group 07.1 includes maritime or continental coastal areas covered by variable thicknesses of sand. These sands are often fixed by psammophilous vegetation and are located mainly in coastal sandy belts and plains, especially in Rocha and Maldonado, as well as sandy coastal areas in Canelones, Montevideo, San Jose, and Colonia. The group also includes sandy dunes near the Negro and Yi rivers.

The soils and sands associated with this group have very low fertility and generally excessive drainage, although some depressed areas may have poor or very poor drainage. Near the coast, vegetation is mainly psammophilous, while inland areas may include summer grassland vegetation and more open ordinary grassland.

From an agricultural perspective, this group has very limited productive capacity. The official CONEAT Productivity Index for group 07.1 is 4, which is far below the national average of 100. The official description mentions that these areas may include seaside resorts, maritime pine plantations, and very limited pastoral use.

For this portfolio map, the `SC = 07.1` highlight should therefore be interpreted as a spatial view of very low-productivity sandy areas, not as a general agricultural opportunity zone.
Source: MGAP / CONEAT, "Descripcion de Grupos de Suelos C.O.N.E.A.T.", group 07.1.

## Next Step

Choose a focused study area for the next Project 02 map, preferably Rocha or Maldonado, because the official group 07.1 description mentions those coastal sandy areas.
