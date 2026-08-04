# University of Toronto (university-of-toronto)

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

The University of Toronto is Canada's leading public research university, ranked #26 in the QS World University Rankings 2025. Its public developer and API footprint is modest and decentralized, centered on the University of Toronto Libraries' TSpace institutional repository (hosted on the Scholaris DSpace platform) plus historical community open-data work. This repository catalogs that footprint as an APIs.json provider profile.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-toronto-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research
- Open Data
- Canada
- Library
- Institutional Repository

## APIs

- **TSpace Institutional Repository (OAI-PMH)** — OAI-PMH 2.0 metadata harvesting endpoint for the UofT Libraries institutional repository on Scholaris/DSpace. Docs: https://utoronto.scholaris.ca/server/oai/request?verb=Identify
- **TSpace DSpace REST API** — Standard DSpace REST API surface for the TSpace repository. Docs: https://utoronto.scholaris.ca/server/api
- **Cobalt Open Data API (deprecated)** — Community open-data REST APIs for UofT courses, buildings, textbooks, food, athletics, exams, parking, and shuttles. Deprecated/archived since 2020. Docs: https://github.com/cobalt-uoft/documentation

## Plans

- [plans/university-of-toronto-plans-pricing.yml](plans/university-of-toronto-plans-pricing.yml)

## Rate Limits

- [rate-limits/university-of-toronto-rate-limits.yml](rate-limits/university-of-toronto-rate-limits.yml)

## FinOps

- [finops/university-of-toronto-finops.yml](finops/university-of-toronto-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.utoronto.ca/
- GitHub: https://github.com/utoronto
- SourceCode (Libraries): https://github.com/utlib
- LinkedIn: https://www.linkedin.com/school/university-of-toronto/
- Plans: plans/university-of-toronto-plans-pricing.yml
- RateLimits: rate-limits/university-of-toronto-rate-limits.yml
- FinOps: finops/university-of-toronto-finops.yml
- Review: review.yml

## Notes

- All cataloged endpoints were probed on 2026-06-03. TSpace OAI-PMH and the DSpace REST API root returned HTTP 200 on the Scholaris platform (`utoronto.scholaris.ca`); `tspace.library.utoronto.ca` redirects there.
- The official EASI Timetable Builder (`ttb.utoronto.ca`) has no publicly documented developer API; guessed endpoint paths returned 404 and were intentionally not cataloged to avoid fabrication.
- Cobalt is included for historical completeness only — it is deprecated/archived since 2020 and unmaintained.
- No official institution-branded developer portal, sign-up flow, or published plans/rate-limit pages were found.

## Maintainers

- Kin Lane — kin@apievangelist.com
