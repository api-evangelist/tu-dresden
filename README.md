# TU Dresden (tu-dresden)

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
