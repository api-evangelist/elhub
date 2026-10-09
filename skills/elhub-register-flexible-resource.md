---
name: elhub-register-flexible-resource
description: Register a controllable unit and its technical resources in the Norwegian Flexibility Information System and group it into a service providing group.
api: elhub:flex-information-system-main-api
spec: openapi/elhub-flex-information-system-main-api-openapi.yml
operations:
- call_controllable_unit_lookup
- create_controllable_unit
- create_technical_resource
- create_service_providing_group
- create_service_providing_group_membership
- read_controllable_unit
generated: '2026-10-09'
method: generated
---

# Register a controllable unit and its technical resources in the Norwegian Flexibility Information System and group it into a service providing group.

## Steps

1. Get a token from the FIS Auth API (`call_token`, separate contract).
2. Check for an existing unit with `call_controllable_unit_lookup`.
3. Create it with `create_controllable_unit` and add `create_technical_resource` entries.
4. Create a group with `create_service_providing_group` and add the unit via `create_service_providing_group_membership`.
5. Confirm with `read_controllable_unit`.

## Rules

Bearer token required. Servers in the contract are test/internal hosts.
