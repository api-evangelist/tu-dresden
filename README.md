# TU Dresden (tu-dresden)

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

Technische Universität Dresden (TU Dresden) is one of Germany's leading research universities (QS World University Rankings 2025 #234), located in Dresden, Saxony. This repository catalogs its public developer/API footprint as an [APIs.json](http://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tu-dresden-api-evangelist&utm_content=repo

## Type

Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, Library, Germany

## APIs

- **TU Dresden Lecture Catalog API** — Gated JSON API for the lecture directory (courses, instructors, buildings, semesters). Requires an API account and auth_code; minimum 10s between calls. Docs: https://vvz.phil.tu-dresden.de/api
- **TU Dresden Shibboleth Single Sign-On (SAML IdP)** — ZIH-operated SAML 2.0 identity provider for federated authentication. Docs: https://idp.tu-dresden.de/docu/ — Metadata: https://idp.tu-dresden.de/idp/shibboleth
- **Qucosa OAI-PMH (TU Dresden Document Server)** — OAI-PMH 2.0 metadata harvesting for the Qucosa publication server (tud.qucosa.de). Base: https://tud.qucosa.de/oai/
- **OpARA Research Data Repository** — ZIH research-data repository for TU Dresden and TU Bergakademie Freiberg. Docs: https://tu-dresden.de/zih/forschung/projekte/opara — Home: https://opara.zih.tu-dresden.de/
- **SLUB Dresden Linked Open Data API** — Documented bibliographic/authority LOD API (Swagger UI) from the Saxony State and University Library serving TU Dresden. Docs: https://data.slub-dresden.de/doc/swagger_api — Source: https://github.com/slub/data.slub-dresden.de

## Plans

[plans/tu-dresden-plans-pricing.yml](plans/tu-dresden-plans-pricing.yml)

## Rate Limits

[rate-limits/tu-dresden-rate-limits.yml](rate-limits/tu-dresden-rate-limits.yml)

## FinOps

[finops/tu-dresden-finops.yml](finops/tu-dresden-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://tu-dresden.de/
- GitHub: https://github.com/tu-dresden
- LinkedIn: https://de.linkedin.com/school/tu-dresden/
- Plans: plans/tu-dresden-plans-pricing.yml
- Rate Limits: rate-limits/tu-dresden-rate-limits.yml
- FinOps: finops/tu-dresden-finops.yml
- Review: review.yml

## Notes

All entries were verified against live HTTP probes on 2026-06-03; no endpoints were fabricated. The lecture-catalog API is gated (account + auth_code required) and rate-limited. The official `github.com/tu-dresden` org exists but is effectively inactive (a single repository last updated in 2015). The SLUB Dresden Linked Open Data API is provided by the Saxony State and University Library, a separate institution that serves TU Dresden, included here for completeness of the university's developer-facing surface. The LinkedIn page returns HTTP 999 due to LinkedIn bot-blocking but is a valid live page.

## Maintainers

- Kin Lane — kin@apievangelist.com
