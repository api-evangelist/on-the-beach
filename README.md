# On the Beach

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

On the Beach Group plc (LSE: OTB) is a Manchester-headquartered online travel agent and the United Kingdom's largest online short-haul beach package holiday specialist, founded in 2004 by Simon Cooper and registered at Aeroworks, 5 Adair Street, Manchester M1 2NQ. It sits on the demand side of the travel distribution chain: an asset-light dynamic packager that buys real-time seats from 42 airlines and hotel inventory from bedbanks and direct hotel contracts, combines them into ATOL-protected packages, and sells them direct to UK and Republic of Ireland consumers through onthebeach.co.uk, sunshine.co.uk and its mobile app. FY25 total transaction value was GBP 1.25bn across 1.7 million customers. It is a consumer of other operators' distribution APIs rather than a publisher of its own - it was the first UK OTA to take a direct NDC connection to Emirates' Online B2B API in 2019 and signed a direct Ryanair "Approved OTA" partnership in 2024 - and it explicitly bypasses the GDS layer entirely. Its API posture as a producer is almost non-existent. The FY25 results describe an "API-first microservices architecture" and a proprietary Hotel Discovery Cache managing more than 5 billion hotel prices, but none of that surface is published: there is no developer portal, no API documentation, no OpenAPI or other machine-readable contract, no partner or trade API, and no self-serve access of any kind. Its only remaining B2B channel, Classic Collection, was put into orderly wind-down on 23 September 2025. The single exception, and the first externally addressable machine surface the company has ever shipped, is a ChatGPT App launched on 1 April 2026 - claimed as the first by a UK OTA - which serves live, bookable package combinations to ChatGPT users over MCP. That surface is distribution-gated rather than developer-facing: no endpoint, tool list, schema, auth flow or terms are documented, and a deliberate mcp.onthebeach.co.uk host exists but is Cloudflare WAF-blocked to every probe.

**Areas:** Travel · United Kingdom · OTA · Online Travel Agency · Booking · Package Holidays · Aviation · Airlines · Distribution · NDC · Hotels · Hospitality

## On the Beach on APIs.io

Everything profiled for On the Beach is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/on-the-beach/](https://apis.io/providers/on-the-beach/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [On the Beach](https://apis.io/servers/on-the-beach/on-the-beach/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [On The Beach Domain Security](https://apis.io/security/on-the-beach/on-the-beach-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.onthebeachgroupplc.com/)
- [Support](https://help.onthebeach.co.uk/hc/en-gb)
- [Terms of service](https://www.onthebeach.co.uk/terms-and-conditions)
- [Privacy policy](https://www.onthebeach.co.uk/privacy)
- [GitHub](https://github.com/onthebeach)

## API Evangelist rating

**Kin Score 10.3** — minimal · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 51.7 |
| Contract quality | 0.0 |
| Contract governance | 0.0 |
| Operational transparency | 2.6 |
| Developer ergonomics | 4.8 |
| Access clarity | 21.1 |

**Agent readiness 3.5** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 12.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/on-the-beach/](https://apis.io/providers/on-the-beach/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for On the Beach: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/on-the-beach/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
