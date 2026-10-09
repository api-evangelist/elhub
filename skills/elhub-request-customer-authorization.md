---
name: elhub-request-customer-authorization
description: Request and track an end customer authorization (consent) via the Elhub Access API, then read the resulting grant and its scopes.
api: elhub:access-api
spec: openapi/elhub-access-api-openapi.yml
operations:
- createV1AuthorizationRequest
- getV1AuthorizationRequest
- listV0AuthorizationGrants
- getV1AuthorizationGrant
- listV0AuthorizationGrantScopes
generated: '2026-10-09'
method: generated
---

# Request and track an end customer authorization (consent) via the Elhub Access API, then read the resulting grant and its scopes.

## Steps

1. Create the request with `createV1AuthorizationRequest`.
2. Poll `getV1AuthorizationRequest` until the end user has acted on it.
3. Find the resulting grant with `listV0AuthorizationGrants`, read it with `getV1AuthorizationGrant`.
4. List what the grant allows with `listV0AuthorizationGrantScopes`.

## Rules

Bearer token (http bearer) required. POST is not marked idempotent in the contract; do not blindly retry createV1AuthorizationRequest.
