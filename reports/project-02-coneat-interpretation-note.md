# Project 02 Interpretation Note - CONEAT Soil Groups

Date: 2026-06-24

## Map Outputs Reviewed

- `projects/02-coneat-soil-mapping/coneat-soil-groups-day-007.png`
- `projects/02-coneat-soil-mapping/coneat-sample-area-day-008.png`

## What The Map Shows

The map shows Uruguay CONEAT soil group polygons from the official MGAP soil service. The `SC` field is used as the classification field, so each color represents a different CONEAT soil group code.

The full-country map proves that the official CONEAT layer can be loaded, styled, and exported from QGIS. The sample-area map is more readable because it zooms into a smaller area and makes the spatial pattern of soil group variation easier to see.

## What `SC` Represents In This Workflow

In this QGIS workflow, `SC` is treated as the main visible soil group/code field in the CONEAT layer. It is useful for categorizing the polygons and making the first soil group map.

At this stage, `SC` should be described as a soil group/code field, not as a direct productivity score unless the official field documentation confirms that relationship.

## Early Interpretation

The sample map shows strong spatial variation in CONEAT soil group codes. This suggests that a land-suitability workflow should not treat the area as uniform. Different polygons may require different interpretation once the official meaning of each `SC` code is documented.

The current output is a mapping and data-loading milestone. It is not yet a decision-support map.

## What The Map Cannot Prove Yet

- It cannot identify the best agricultural land without official interpretation of each CONEAT group.
- It cannot make farm purchase, legal, valuation, or soil-management recommendations.
- It does not include slope, water access, roads, land use, rainfall, or field validation.
- It does not yet compare productivity classes or calculate area by group.
- It uses a sample zoomed area, not a formally selected department or study boundary.

## Next GIS Questions

1. What does each `SC` code mean in the official CONEAT documentation?
2. Is there a field or table that links CONEAT groups to productivity index values?
3. Which official department or study area should be used for a cleaner case study?
4. Can QGIS calculate area by `SC` group for the selected study area?
5. Should the next map show all `SC` groups or simplified classes?

## Next Practical Step

Choose an official study area, preferably a department or smaller agricultural region, then clip or filter the CONEAT layer to that area before creating the next map.
