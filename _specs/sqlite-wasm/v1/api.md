---
layout: spec
title: sqlite wasm — API
nav_title: "API"
nav_order: 30
---
# API
## Overview
- Audience & usage; versioning policy

## Base Info
- **Base URL:** `https://api.example.com`
- **Auth:** Bearer / API key / OAuth2
- **Content-Type:** `application/json`
- **Rate limits / Pagination / Idempotency**
- **Webhooks** (delivery, retries, signatures)

## Errors
```json
{ "error": { "code": "RESOURCE_NOT_FOUND", "message": "…", "details": {} } }
```

## Endpoints
### GET /v1/things
- Params: `page`, `limit`
- Response:
```json
{ "items": [], "next": "…" }
```
- Sample:
```bash
curl -H "Authorization: Bearer $TOKEN" \
     "https://api.example.com/v1/things?limit=20"
```

## Webhooks (if any)
- …

## SDK Mapping
- …
