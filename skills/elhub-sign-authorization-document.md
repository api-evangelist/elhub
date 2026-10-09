---
name: elhub-sign-authorization-document
description: Create an authorization document in Elhub, fetch it as PDF for signing, and submit the signed PDF.
api: elhub:access-api
spec: openapi/elhub-access-api-openapi.yml
operations:
- createV1AuthorizationDocument
- getV0AuthorizationDocumentPdf
- submitV0AuthorizationDocument
- getV1AuthorizationDocument
generated: '2026-10-09'
method: generated
---

# Create an authorization document in Elhub, fetch it as PDF for signing, and submit the signed PDF.

## Steps

1. Create the document with `createV1AuthorizationDocument`.
2. Download the PDF with `getV0AuthorizationDocumentPdf`.
3. Upload the signed PDF with `submitV0AuthorizationDocument` (PUT /access/v0/authorization-documents/{id}.pdf).
4. Check status with `getV1AuthorizationDocument`.

## Rules

Bearer token required.
