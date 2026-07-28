# On the Beach (on-the-beach)

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

No public APIs are listed. On the Beach Group publishes no developer portal, no API documentation, and no machine-readable API contract. Every developer subdomain (`developer.`, `api.`, `docs.`) fails to resolve, and `/openapi.json`, `/llms.txt` and `/.well-known/*` return HTTP 404 on the consumer host. See [review.yml](review.yml) for the full probe log.

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

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
