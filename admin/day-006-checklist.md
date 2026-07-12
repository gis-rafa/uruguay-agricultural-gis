# Day 6 Checklist - CONEAT Layer Load

Date: 2026-06-23

## Goal

Start Project 02 by loading the official CONEAT soil group layer into QGIS and documenting the source.

## Today's Main Objective

Move from a basic Uruguay boundary map to real Uruguay soil-productivity data.

## Do Today

- [x] Open the main QGIS project.
- [x] Add an ArcGIS REST connection named `MGAP Suelos`.
- [x] Use the official MGAP Suelos service URL.
- [x] Load the feature version of `Grupos CONEAT (1:40.000)`.
- [x] Confirm the layer appears on the map.
- [x] Open the attribute table.
- [x] Record the feature count.
- [x] Record visible fields.
- [x] Rename the layer to `CONEAT Soil Groups`.
- [x] Style the layer by the `SC` field using categorized symbology.
- [x] Save the QGIS project.

## Source Notes

```text
Source name: Grupos CONEAT (1:40.000)
Provider: MGAP / Uruguay official ArcGIS REST service
URL: https://mapas.mgap.gub.uy/arcgis/rest/services/SNIA_Temas/Suelos/MapServer
Feature count: 33,557
Main useful field: SC
Example SC values: 07.1, 07.2, 2.21, 3.15, 3.12
Other fields: OBJECTID, Shape.STArea(), Shape.STLength()
Loaded in QGIS: yes
```

## Minimum Win

The official CONEAT layer is loaded, visible, inspected, renamed, saved, and documented.

## Next Task

Create the first draft CONEAT soil group map layout and export a PNG/PDF preview.
