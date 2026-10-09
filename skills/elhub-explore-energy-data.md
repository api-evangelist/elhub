---
name: elhub-explore-energy-data
description: Look up open Elhub reference data (price areas, grid areas, municipalities, parties, metering points) through the public Energy Data API.
api: elhub:energy-data-api
spec: openapi/elhub-energy-data-api-openapi.yml
operations:
- price_areas
- grid_areas
- municipalities
- parties
- metering_points
- metering_points_id
generated: '2026-10-09'
method: generated
---

# Look up open Elhub reference data (price areas, grid areas, municipalities, parties, metering points) through the public Energy Data API.

## Steps

1. Call `price_areas` / `grid_areas` / `municipalities` to list the reference datasets (GET /energy-data/v0/...).
2. Use `parties` to resolve market parties (grid companies, suppliers).
3. Use `metering_points` to filter metering points, then `metering_points_id` for one record.

## Rules

The contract declares no security scheme; the description says V0 is accessible to the public. Read-only (GET), so retries are safe.
