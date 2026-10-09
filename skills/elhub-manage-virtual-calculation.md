---
name: elhub-manage-virtual-calculation
description: Create a shared-production virtual calculation and manage its versions via the Elhub Settlement Virtual Calculations API.
api: elhub:settlement-virtual-calculations-api
spec: openapi/elhub-settlement-virtual-calculations-api-openapi.yml
operations:
- createVirtualCalculation
- getVirtualCalculation
- createSharedProductionVersion
- getAllVersionsByUdcId
- updateSharedProductionVersion
- subscribeToResourceChanges
generated: '2026-10-09'
method: generated
---

# Create a shared-production virtual calculation and manage its versions via the Elhub Settlement Virtual Calculations API.

## Steps

1. Create with `createVirtualCalculation`, read back with `getVirtualCalculation`.
2. Add a version with `createSharedProductionVersion`; list versions with `getAllVersionsByUdcId`; amend with `updateSharedProductionVersion`.
3. Follow changes with `subscribeToResourceChanges` (GET .../events).

## Rules

Bearer token named `maskinporten` in the contract (Maskinporten-issued). Do not blindly retry POSTs.
