# On the Beach (on-the-beach)

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

On the Beach Group plc (LSE: OTB) is a Manchester-headquartered online travel agent and the United Kingdom's largest online short-haul beach package holiday specialist, founded in 2004 by Simon Cooper and registered at Aeroworks, 5 Adair Street, Manchester M1 2NQ. It sits on the demand side of the travel distribution chain: an asset-light dynamic packager that buys real-time seats from 42 airlines and hotel inventory from bedbanks and direct hotel contracts, combines them into ATOL-protected packages, and sells them direct to UK and Republic of Ireland consumers through onthebeach.co.uk, sunshine.co.uk and its mobile app. FY25 total transaction value was GBP 1.25bn across 1.7 million customers. It is a consumer of other operators' distribution APIs rather than a publisher of its own — it was the first UK OTA to take a direct NDC connection to Emirates' Online B2B API in 2019 and signed a direct Ryanair "Approved OTA" partnership in 2024 — and it explicitly bypasses the GDS layer entirely. Its API posture as a producer is honestly non-existent. The FY25 results describe an "API-first microservices architecture" and a proprietary Hotel Discovery Cache managing more than 5 billion hotel prices, but none of that surface is published: there is no developer portal, no API documentation, no OpenAPI or other machine-readable contract, no partner or trade API, and no self-serve access of any kind. Its only remaining B2B channel, Classic Collection, was put into orderly wind-down on 23 September 2025. Public docs do not exist, there is no published exit path, and every probed developer subdomain and contract path returned 404 or did not resolve.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/on-the-beach/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/on-the-beach/refs/heads/main/apis.yml)

## Tags

- Travel
- United Kingdom
- OTA
- Online Travel Agency
- Booking
- Package Holidays
- Aviation
- Airline
- Distribution
- NDC
- Hotels
- Hospitality

## Timestamps

- **Created:** 2026-07-28
- **Modified:** 2026-07-28

## APIs

No public APIs are listed. On the Beach Group publishes no developer portal, no API documentation, and no machine-readable API contract. Every developer subdomain (`developer.`, `api.`, `docs.`) fails to resolve, and `/openapi.json` and `/llms.txt` do not exist on any host. See [review.yml](review.yml) for the full probe log.

**One exception, found on 2026-07-28.** On the Beach launched a **ChatGPT App on 1 April 2026** — reported as the first by a UK OTA — which serves live, bookable holiday package combinations to ChatGPT users conversationally, with a booking deep link back to onthebeach.co.uk. ChatGPT Apps are served over **MCP**, making this the first externally addressable machine surface the company has ever shipped, and the delivery of the "direct integration into ChatGPT, Gemini, and emerging AI platforms" its FY25 results promised. It is distribution-gated, not developer-facing: no endpoint, tool list, input schema, auth flow, rate limit or terms is documented. A deliberate `mcp.onthebeach.co.uk` host exists (real DNS record, valid TLS, not a wildcard) but every request — including `tools/list` — is answered by the Cloudflare WAF with HTTP 403, so no tool was captured. See [mcp/on-the-beach-mcp.yml](mcp/on-the-beach-mcp.yml).

Certificate transparency shows the private side of the same architecture: certificates issued for `api.onthebeach.co.uk`, `api.sandbox1-8.onthebeach.co.uk`, `uapi.sandbox1-8.onthebeach.co.uk` and `otb-payments-notifications-api.staging.onthebeach.co.uk` — all of which now return NXDOMAIN to public DNS.

## Artifacts

| Artifact | File | Method |
| --- | --- | --- |
| MCP server | [mcp/on-the-beach-mcp.yml](mcp/on-the-beach-mcp.yml) | searched + probed |
| Well-known | [well-known/on-the-beach-well-known.yml](well-known/on-the-beach-well-known.yml) | searched |
| Packages | [packages/on-the-beach-packages.yml](packages/on-the-beach-packages.yml) | searched |
| llms.txt | [llms/on-the-beach-llms.txt](llms/on-the-beach-llms.txt) | generated |
| Domain security | [security/on-the-beach-domain-security.yml](security/on-the-beach-domain-security.yml) | probed |

## Switching Cost

| Dimension | Finding |
| --- | --- |
| Interface shape | `none-published` — no NDC, OpenTravel/OTA, HTNG, OpenAPI or partner XML published |
| Second source | `interchangeable-alternatives` — Jet2holidays, TUI UK, easyJet holidays, loveholidays, Expedia |
| Exit path | `no-export-published` — no export operation; privacy notice unreachable (HTTP 403) |
| Identifier portability | IATA airline/airport codes and CAA ATOL certificates inbound; proprietary internal inventory IDs otherwise |
| Contractual lock-in | Nothing published — no developer or partner agreement exists |
| Access gate | `none-published` — nothing to sign up for |
| Distribution model | `aggregator-reseller` — direct-to-consumer only, no GDS, no channel manager, B2B closed September 2025 |
| NDC posture | NDC consumer, not provider — Emirates Online B2B direct connect (2019), Ryanair Approved OTA (2024) |

## Common Properties

- [Website](https://www.onthebeachgroupplc.com/)
- [Consumer Website](https://www.onthebeach.co.uk/)
- [About](https://www.onthebeachgroupplc.com/about-us/who-we-are)
- [Strategy](https://www.onthebeachgroupplc.com/about-us/strategy)
- [Investor Relations](https://www.onthebeachgroupplc.com/investor-centre)
- [Annual Report](https://www.onthebeachgroupplc.com/~/media/Files/O/On-The-Beach/investor-docs/results-and-presentations/on-the-beach-group-final-results-2025.pdf)
- [GitHub Organization](https://github.com/onthebeach)
- [LinkedIn](https://www.linkedin.com/company/on-the-beach)
- [Contact](https://www.onthebeachgroupplc.com/contact)
- [Support (Zendesk help centre)](https://help.onthebeach.co.uk/hc/en-gb)
- [Terms of Service](https://www.onthebeach.co.uk/terms-and-conditions)
- [Privacy Policy](https://www.onthebeach.co.uk/privacy)
- [Affiliate Program (Partnerize / Awin)](https://www.onthebeach.co.uk/affiliates)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
