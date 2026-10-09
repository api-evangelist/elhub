---
name: elhub-export-energy-data
description: List and download Elhub energy data export files through the Data Export API.
api: elhub:data-export-api
spec: openapi/elhub-data-export-api-openapi.yml
operations:
- energy_data
- energy_data_file_id
generated: '2026-10-09'
method: generated
---

# List and download Elhub energy data export files through the Data Export API.

## Steps

1. List available exports with `energy_data`.
2. Download a file with `energy_data_file_id`.

## Rules

Read-only GETs. Two operations in this contract lack an operationId; the overlay adds derived ones.
