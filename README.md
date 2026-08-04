# BizVerify

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
- **User-agent gate** — the spec returns HTTP 403 to `Python-urllib` while serving curl, an empty
  UA, and `python-requests` normally. Narrow, but enough to silently starve a urllib-based
  harvester.

## This is a catalog entry, not BizVerify

This repo is API Evangelist's profile *about* BizVerify. For the product, an API key, or support,
go to [bizverify.co](https://bizverify.co).

If something here is wrong, open an issue on this repo or in the
[APIs.io Inbox](https://github.com/api-search/inbox).
