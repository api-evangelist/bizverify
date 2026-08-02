# BizVerify

API Evangelist catalog entry for [BizVerify](https://bizverify.co) — business entity verification
(KYB) for AI agents and developer workflows. Confirms business registrations, status, good
standing and public company details across supported US and international jurisdictions.

## What they ship

| | |
|---|---|
| REST API | OpenAPI 3.0.3 — 20 paths, 21 operations |
| MCP server | **Hosted**, Streamable HTTP, 9 tools, `tools/list` answers unauthenticated |
| Auth | `X-API-Key` header or bearer token |
| Agent surface | `llms.txt`, RFC 9727 API catalog, per-vendor tool manifests for OpenAI and Anthropic |

The agent-readable surface is well ahead of most providers this size — a real
`application/linkset+json` API catalog is rare, and shipping `/tools/openai.json` and
`/tools/anthropic.json` alongside MCP is rarer still.

## Known gaps in the published contract

Recorded in `apis.yml` under `x-evidence.defects_found`, and reported to the provider:

- **`servers: []`** — the OpenAPI declares no server, so it is not callable as published. The base
  URL here comes from the API catalog linkset and the live host.
- **No schemas** — 21 operations with no `components.schemas`, so request and response bodies are
  undescribed.
- **User-agent gate** — the spec returns HTTP 403 to a default Python client while serving curl
  normally. Automated consumers using a stock library UA are blocked.

## This is a catalog entry, not BizVerify

This repo is API Evangelist's profile *about* BizVerify. For the product, an API key, or support,
go to [bizverify.co](https://bizverify.co).

If something here is wrong, open an issue on this repo or in the
[APIs.io Inbox](https://github.com/api-search/inbox).
