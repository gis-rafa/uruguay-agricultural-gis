# Day 10 Checklist - CONEAT Group 07.1 Highlight

Date: 2026-06-24

## Goal

Create a clearer analytical map by filtering the CONEAT layer to one soil group code.

## Today's Main Objective

Show how a single CONEAT group can be isolated and mapped in QGIS.

## Do Today

- [x] Duplicate `CONEAT Soil Groups`.
- [x] Rename duplicate to `CONEAT Group 07.1`.
- [x] Apply filter: `"SC" = '07.1'`.
- [x] Turn off the full CONEAT layer.
- [x] Make `Uruguay Boundary` transparent.
- [x] Style `CONEAT Group 07.1` with stronger fill and outline.
- [x] Create layout: `CONEAT Group 07.1 Highlight`.
- [x] Add map, title, source note, north arrow, and scale bar.
- [x] Export PNG.
- [x] Export PDF.

## Outputs

- `projects/02-coneat-soil-mapping/coneat-group-07-1-highlight-day-009.png`
- `projects/02-coneat-soil-mapping/coneat-group-07-1-highlight-day-009.pdf`

## Quality Notes

- This highlight map is clearer than the full categorized CONEAT map.
- It demonstrates filtering by the `SC` field.
- It should not claim what group `07.1` means until official CONEAT documentation is checked.

## Minimum Win

One filtered CONEAT group map exported as PNG and PDF.

## Next Task

Write a short interpretation note for the `SC = 07.1` highlight map.
