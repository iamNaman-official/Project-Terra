# Source Code

Reusable and validated code extracted from successful experiments.

## Purpose

Code should generally move here after it has been:

1. Experimented with
2. Tested
3. Validated
4. Documented
5. Refactored into reusable components

## Structure

- `data/` — Data ingestion, loading, and validation
- `analysis/` — Statistical analysis and trend detection
- `ml/` — Machine learning components
- `gis/` — Spatial and geospatial processing
- `visualization/` — Reusable visualization components

## Principle

Do not put every experiment directly into `src/`.

Use:

`experiments/` → validation → `src/`

This keeps experimental work separate from reusable code.