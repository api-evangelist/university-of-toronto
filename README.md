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

The University of Toronto is Canada's largest public research university, with three campuses in the Greater Toronto Area. Like almost every institution its size it is a **federation of buyers rather than a producer of APIs**, and this profile is deliberate about which side of that line each surface falls on. Two surfaces are genuinely institution-operated, both on `utoronto.ca`; three more are real institutional relationships running on someone else's contract and are labelled `tenant` rather than credited to the University. This repository catalogs that footprint as an APIs.json provider profile.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-toronto-api-evangelist&utm_content=repo

## Type

- university / Public Research University — Index / Consumer / 3rd-Party

## Tags

- University
- Higher Education
- Education
- Canada
- U15
- Research
- Course Catalog
- Identity Federation
- Research Data
- Institutional Repository
- Library
- Public Research University

## APIs

Every entry carries an operator. `institution` means the University runs the thing the contract describes; `tenant` means the data is the University's and the contract is a vendor's.

- **Timetable Builder API** — `institution` — `https://api.easi.utoronto.ca/ttb`. Live, unauthenticated course, section, meeting-time, enrolment and building data for all divisions and all three campuses, operated by Enterprise Applications and Solutions Integration (EASI) within U of T Information Technology Services. Six operations verified live 2026-08-19. No documentation, no OpenAPI, no terms of use published by the University. Docs: https://ttb.utoronto.ca/
- **UTORauth Shibboleth Identity Provider** — `institution` — `https://idpz.utorauth.utoronto.ca/idp/shibboleth`. Signed SAML 2.0 metadata registered in the Canadian Access Federation, asserting the REFEDS Research & Scholarship entity category and SIRTFI assurance.
- **TSpace Institutional Repository (OAI-PMH)** — `tenant` — `https://utoronto.scholaris.ca/server/oai/request`. The repository is U of T Libraries'; the endpoint runs on Scholaris, the OCUL-operated DSpace service.
- **TSpace DSpace REST API** — `tenant` — `https://utoronto.scholaris.ca/server/api`. Stock DSpace 8.4 HAL API shipped by the Scholaris platform.
- **U of T Dataverse (Borealis)** — `tenant` — collection `toronto` inside Borealis, the Canadian Dataverse Repository operated by Scholars Portal. Deliberately carries no base URL: `borealisdata.ca` is a shared vendor host.

## Artifacts

- [openapi/university-of-toronto-timetable-builder-openapi.yml](openapi/university-of-toronto-timetable-builder-openapi.yml) — observation-derived, **not** a University of Toronto artifact
- [json-schema/](json-schema/) · [examples/](examples/) · [vocabulary/](vocabulary/) · [rules/](rules/) · [json-ld/](json-ld/)
- [authentication/](authentication/) · [scopes/](scopes/) · [errors/](errors/) · [conformance/](conformance/) · [lifecycle/](lifecycle/)

## Plans

- [plans/university-of-toronto-plans-pricing.yml](plans/university-of-toronto-plans-pricing.yml)

## Rate Limits

- [rate-limits/university-of-toronto-rate-limits.yml](rate-limits/university-of-toronto-rate-limits.yml)

## FinOps

- [finops/university-of-toronto-finops.yml](finops/university-of-toronto-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Common Properties

- Website: https://www.utoronto.ca/
- LLMsTxt: https://www.utoronto.ca/llms.txt
- CourseCatalog: https://ttb.utoronto.ca/
- IdentityFederation: https://idpz.utorauth.utoronto.ca/idp/shibboleth
- ResearchRepository: https://utoronto.scholaris.ca/
- LibraryCatalog: https://onesearch.library.utoronto.ca/
- ResearchComputing: https://docs.scinet.utoronto.ca/
- AIPolicy: https://ai.utoronto.ca/
- AITooling: https://its.utoronto.ca/ai/
- OpenData: https://data.utoronto.ca/
- Documentation: https://easi.its.utoronto.ca/
- PrivacyPolicy: https://www.utoronto.ca/privacy
- Status: https://www.utoronto.ca/campus-status
- Blog: https://www.utoronto.ca/news
- Support: https://www.utoronto.ca/contacts
- GitHubOrganization: https://github.com/utoronto
- SourceCode (Libraries): https://github.com/utlib
- LinkedIn: https://www.linkedin.com/school/university-of-toronto/

## Notes

- Re-profiled 2026-08-19 under the university pipeline, with operator attribution settled before anything was saved.
- **The June 2026 review was wrong about the timetable.** It concluded no timetable API could be cataloged because guessed paths under `ttb.utoronto.ca` returned 404. The API is real; it lives at `https://api.easi.utoronto.ca/ttb` and its operation names are declared in the official client bundle.
- The **U of T Dataverse in Borealis** was added as a tenant relationship. `borealisdata.ca` is a shared host claimed by several Canadian institutions, so no base URL is published for it here.
- The deprecated community **Cobalt** open-data API was **removed**. `https://cobalt.qas.im/1.0/courses` returns HTTP 404 and the project was never institution-operated.
- `https://onesearch.library.utoronto.ca/api/search` returns HTTP 200 with the site's Next.js shell — a soft 404, not an API. Not cataloged.
- `developer.utoronto.ca` and `api.utoronto.ca` are NXDOMAIN. There is no developer portal and no central API host.
- No `.well-known/security.txt`, no OpenAPI, no Swagger UI, no terms of use for any API, no versioning scheme, no status page for developers, no rate-limit statement, no OAuth surface.
- The University **does** publish an `llms.txt` at its web root — 4.4 KB of curated, authoritative links. That is more agent-facing provision than most of this cohort makes.
- Five operations declared in the shipping Timetable Builder client return 404 from the deployed gateway. Operations are withdrawn without notice; only live-verified operations are described in the OpenAPI.

## Maintainers

- Kin Lane — kin@apievangelist.com
