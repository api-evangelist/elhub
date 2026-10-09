---
name: elhub-manage-contracts
description: Read and maintain metering-point contracts through the Elhub Market Data Contracts JSON:API.
api: elhub:market-data-contracts-api
spec: openapi/elhub-market-data-contracts-api-openapi.yml
operations:
- getContracts
- getContractById
- createContracts
- patchContractById
- summary
generated: '2026-10-09'
method: generated
---

# Read and maintain metering-point contracts through the Elhub Market Data Contracts JSON:API.

## Steps

1. List with `getContracts`, read one with `getContractById`, get counts with `summary`.
2. Create with `createContracts`; amend with `patchContractById`.

## Rules

Bearer token required. JSON:API document format.
