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

Technische Universität Dresden (TU Dresden) is one of Germany's leading research universities (QS World University Rankings 2025 #234), located in Dresden, Saxony. This repository catalogs its public developer/API footprint as an [APIs.json](http://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tu-dresden-api-evangelist&utm_content=repo

## Type

Index / Provider / Private — `x-type: university`, `x-category: Technical University`

## Tags

University, Higher Education, Education, Germany, Saxony, TU9, Research, Research Data, Research Computing, Artificial Intelligence, Identity Federation, OAI-PMH, Institutional Repository, Open Access

## APIs

Every entry carries an `x-operator` — who runs the thing the entry describes. For a university
that is almost never the same answer as whose name is on the hostname.

- **TUD:AI LLM API** *(institution)* — OpenAI-compatible LLM inference operated by ZIH and ScaDS.AI Dresden/Leipzig on TU Dresden's own network (141.76.0.0/16, netname TUDINF-LAN). Keys from https://selfservice.tu-dresden.de/services/scads-llm-api/. Base: https://llm.scads.ai/v1 — Docs: https://llm.scads.ai/docs/
- **OPARA Research Data Repository REST API** *(institution)* — DSpace 7.6.2 REST API, read-open, operated by ZIH for TU Dresden, TU Bergakademie Freiberg, HTW Dresden and Hochschule Mittweida. Base: https://opara.zih.tu-dresden.de/server/api
- **OPARA OAI-PMH Harvesting Interface** *(institution)* — Twelve metadata prefixes, four institutional set trees. Base: https://opara.zih.tu-dresden.de/server/oai/request
- **TU Dresden Identity Provider (Shibboleth SAML 2.0 + OpenID Connect)** *(institution)* — DFN-AAI registered, exported to eduGAIN, REFEDS R&S + SIRTFI. Now also serves OIDC discovery and a JWKS. Metadata: https://idp.tu-dresden.de/idp/shibboleth
- **TU Dresden Lecture Catalog API (Vorlesungsverzeichnis)** *(institution)* — Gated JSON API for the Faculty of Arts lecture directory; account + `auth_code`, minimum 10s between calls. Docs: https://vvz.phil.tu-dresden.de/api
- **TU Dresden Research Portal (Elsevier Pure) Web Service** *(tenant)* — TU Dresden's CRIS on Elsevier Pure. Portal public; `/ws/api`, `/ws/rest` and `/ws/oai` all 403 to the public internet. Portal: https://fis.tu-dresden.de/portal/
- **Qucosa TU Dresden OAI-PMH** *(tenant)* — TU Dresden's view of the SLUB-operated Saxon document server. Base: https://tud.qucosa.de/oai/

Removed on 2026-08-30: five OpenAPI contracts and five apis[] entries that were all the SLUB
Dresden Linked Open Data API at `data.slub-dresden.de`, plus the twenty-two artifacts derived from
them. SLUB is a separate Saxon state institution with its own Crossref membership and its own
DataCite provider symbol; its API is not TU Dresden's engineering.

## Plans

[plans/tu-dresden-plans-pricing.yml](plans/tu-dresden-plans-pricing.yml)

## Rate Limits

[rate-limits/tu-dresden-rate-limits.yml](rate-limits/tu-dresden-rate-limits.yml)

## FinOps

[finops/tu-dresden-finops.yml](finops/tu-dresden-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://tu-dresden.de/
- Blog: https://tu-dresden.de/tu-dresden/newsportal
- GitHub Organization: https://github.com/tu-dresden
- LinkedIn: https://de.linkedin.com/school/tu-dresden/
- Documentation: https://llm.scads.ai/docs/
- API Reference: https://llm.scads.ai/docs/usage/api/
- Status: https://llm.scads.ai/status/
- Support: https://tu-dresden.de/zih/dienste/service-desk
- Terms of Service: https://tu-dresden.de/impressum
- Privacy Policy: https://tu-dresden.de/datenschutz
- Identity Federation: https://met.refeds.org/met/entity/https%3A%2F%2Fidp.tu-dresden.de%2Fidp%2Fshibboleth/
- Research Repository: https://opara.zih.tu-dresden.de/
- Library Catalog: https://katalog.slub-dresden.de/
- Course Catalog: https://vvz.phil.tu-dresden.de/
- Research Computing: https://tu-dresden.de/zih/hochleistungsrechnen
- AI Policy: https://tu-dresden.de/tu-dresden/digitalisierung/ki-an-der-tu-dresden
- AI Tooling: https://llm.scads.ai/docs/
- Authentication: authentication/tu-dresden-authentication.yml
- Errors: errors/tu-dresden-problem-types.yml
- Conformance: conformance/tu-dresden-education-standards.yml
- Vulnerability Disclosure: security/tu-dresden-vulnerability-disclosure.yml
- Domain Security: security/tu-dresden-domain-security.yml
- Plans: plans/tu-dresden-plans-pricing.yml
- Rate Limits: rate-limits/tu-dresden-rate-limits.yml
- FinOps: finops/tu-dresden-finops.yml
- Review: review.yml

## Notes

Re-profiled 2026-08-30 under the API Evangelist university pipeline, which settles who operates a
surface before crediting it to the institution. Every status code in `apis.yml` `x-coverage` was
observed live on that date with a browser User-Agent; more than sixty hosts and paths were probed
and nothing blocked the pass.

TU Dresden holds conformance against four of the twelve `education`-regime domain standards —
`oai-pmh`, `shibboleth`, `saml` and `datacite` — and all four are institution-operated, which is
unusual in this cohort. See `conformance/tu-dresden-education-standards.yml`. It is not a Crossref
member and exposes no ORCID iD on any machine-readable surface.

TU Dresden publishes no OpenAPI of its own. The only contract served on any of its surfaces is
`https://llm.scads.ai/openapi.json`, which is LiteLLM's generic proxy specification
(`info.title: LiteLLM API`) — the deployment is TU Dresden's, the document is the product's, and it
is deliberately not saved here. No OpenAPI has been authored from probe responses or prose
parameter tables.

Confirmed absent by DNS: `data.tu-dresden.de`, `api.tu-dresden.de`, `opendata.tu-dresden.de`,
`developer.tu-dresden.de`, `gitlab.tu-dresden.de`, `elearning.tu-dresden.de`,
`status.tu-dresden.de`. Confirmed absent by fetch: `https://tu-dresden.de/llms.txt` (404). A
`security.txt` IS published at `https://tu-dresden.de/.well-known/security.txt`. The official
`github.com/tu-dresden` org exists but holds a single repository. The LinkedIn page returns HTTP
999 due to LinkedIn bot-blocking but is a valid live page.

Not TU Dresden's, and recorded as such: OPAL at `bildungsportal.sachsen.de` (the Saxony-wide LMS
run by BPS Bildungsportal Sachsen GmbH) and the Mensa API at `studentenwerk-dresden.de` (the
student services organisation).

## Maintainers

- Kin Lane — kin@apievangelist.com
