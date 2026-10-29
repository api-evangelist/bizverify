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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

BizVerify is a business entity verification (KYB) API built for AI agents as much as for developers. It confirms business registrations, status, good standing and available public company details across supported US and international jurisdictions, through a REST API and a hosted MCP server that exposes the same capability as nine tools. The agent surface is the unusual part for a provider this size: alongside the OpenAPI it publishes an llms.txt, a proper RFC 9727 API catalog served as application/linkset+json, per-vendor tool manifests at /tools/openai.json and /tools/anthropic.json, and an open-source MCP client repository. Access is credit-based with a free-tier allowance, and the MCP server answers tools/list without credentials.

**Areas:** Business Verification · KYB · Entity Verification · Compliance · MCP · Agent-Native · Developer Tools

## BizVerify on APIs.io

Everything profiled for BizVerify is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/bizverify/](https://apis.io/providers/bizverify/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [BizVerify MCP Server](https://apis.io/apis/bizverify/bizverify-mcp-server/) — Hosted MCP server over Streamable HTTP exposing nine tools — get_config, list_jurisdictions, verify_business, search_entities, check_job_status, get_entity,…
- [BizVerify Account API](https://apis.io/apis/bizverify/bizverify-account-api/) — The Account API from BizVerify — 5 operation(s) for account.
- [BizVerify Auth API](https://apis.io/apis/bizverify/bizverify-auth-api/) — The Auth API from BizVerify — 2 operation(s) for auth.
- [BizVerify Billing API](https://apis.io/apis/bizverify/bizverify-billing-api/) — The Billing API from BizVerify — 2 operation(s) for billing.
- [BizVerify Entities API](https://apis.io/apis/bizverify/bizverify-entities-api/) — The Entities API from BizVerify — 2 operation(s) for entities.
- [BizVerify Meta API](https://apis.io/apis/bizverify/bizverify-meta-api/) — The Meta API from BizVerify — 2 operation(s) for meta.
- [BizVerify Public API](https://apis.io/apis/bizverify/bizverify-public-api/) — The Public API from BizVerify — 2 operation(s) for public.
- [BizVerify Search API](https://apis.io/apis/bizverify/bizverify-search-api/) — The Search API from BizVerify — 1 operation(s) for search.
- [BizVerify Tools API](https://apis.io/apis/bizverify/bizverify-tools-api/) — The Tools API from BizVerify — 2 operation(s) for tools.
- [BizVerify Verification API](https://apis.io/apis/bizverify/bizverify-verification-api/) — The Verification API from BizVerify — 2 operation(s) for verification.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [mcp](https://apis.io/servers/bizverify/mcp/)

#### Collections (10)

Postman and Open Collection request collections.

- [BizVerify API](https://apis.io/collections/bizverify/open-bizverify/)
- [BizVerify Account API](https://apis.io/collections/bizverify/open-bizverify-account-api/)
- [BizVerify Auth API](https://apis.io/collections/bizverify/open-bizverify-auth-api/)
- [BizVerify Billing API](https://apis.io/collections/bizverify/open-bizverify-billing-api/)
- [BizVerify Entities API](https://apis.io/collections/bizverify/open-bizverify-entities-api/)
- [BizVerify Meta API](https://apis.io/collections/bizverify/open-bizverify-meta-api/)
- [BizVerify Public API](https://apis.io/collections/bizverify/open-bizverify-public-api/)
- [BizVerify Search API](https://apis.io/collections/bizverify/open-bizverify-search-api/)
- [BizVerify Tools API](https://apis.io/collections/bizverify/open-bizverify-tools-api/)
- [BizVerify Verification API](https://apis.io/collections/bizverify/open-bizverify-verification-api/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://bizverify.co)
- [Documentation](https://docs.bizverify.co)
- [Terms of service](https://bizverify.co/terms)
- [Privacy policy](https://bizverify.co/privacy)

## API Evangelist rating

**Kin Score 26.9** — thin · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 76.7 |
| Contract quality | 41.4 |
| Contract governance | 0.0 |
| Operational transparency | 5.3 |
| Developer ergonomics | 16.0 |
| Access clarity | 34.2 |

**Agent readiness 35.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | unknown |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | distinct |

**Regulatory alignment 7.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/bizverify/](https://apis.io/providers/bizverify/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for BizVerify: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/bizverify/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
