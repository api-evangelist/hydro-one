# Hydro One

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

Hydro One Limited (TSX: H) is Canada's largest electricity transmission and distribution service provider, transmitting and distributing electricity across Ontario — the province the company describes as "home to 38 per cent of Canada's population." It sits in the regulated wires tier of the value chain: it owns and operates the provincial transmission grid and a rural/regional distribution network serving roughly 1.5 million customers, while the Ontario market itself is operated by the IESO and rates are set by the Ontario Energy Board. Its API posture is defined entirely by regulation, not by product. Ontario Regulation 633/21 (Energy Data, under the Electricity Act, 1998) compels Ontario electricity and natural gas distributors to implement Green Button Download My Data (DMD) and Connect My Data (CMD) and to have those implementations certified by the Green Button Alliance. Hydro One publishes DMD as an authenticated XML export inside My Account, runs a live Green Button CMD OAuth 2.0 authorization surface at www.hydroone.com/green-button-cmd-home, and operates a published third-party vendor onboarding form and terms and conditions — but the CMD resource base URI, client credentials, and test accounts are issued privately during onboarding and are not published anywhere. There is no developer subdomain, no OpenAPI or Swagger definition, and no self-serve signup. The split is the finding: consumer energy data is available through a real, standards-based, mandated API that a developer can only reach by application and 90-day connectivity testing, while open grid and market data is entirely absent — Hydro One publishes no open data portal and no documented public system or outage API, leaving Ontario market data to the IESO.

**Areas:** Energy · Canada · Utilities · Electricity · Grid · Smart Metering · Green Button · Energy Data · Transmission · Distribution

## Hydro One on APIs.io

Everything profiled for Hydro One is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/hydro-one/](https://apis.io/providers/hydro-one/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Hydro One Green Button Connect My Data (CMD)](https://apis.io/apis/hydro-one/hydro-one-green-button-connect-my-data/) — Hydro One's Green Button Connect My Data implementation, mandated by Ontario Regulation 633/21. A registered third-party vendor obtains an OAuth 2.0…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Hydro One Authentication](https://apis.io/security/hydro-one/hydro-one-authentication/)
- [Hydro One Domain Security](https://apis.io/security/hydro-one/hydro-one-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Hydro One Scopes](https://apis.io/scopes/hydro-one/hydro-one-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.hydroone.com/)
- [Documentation](https://www.hydroone.com/saving-money-and-energy/green-button)
- [Getting started](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-apps)
- [Sign up](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-onboarding-form)
- [Support](https://www.hydroone.com/contact)
- [Terms of service](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions)
- [Privacy policy](https://www.hydroone.com/privacy)

## API Evangelist rating

**Kin Score 26.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 58.0 |
| Contract quality | 0.0 |
| Contract governance | 18.2 |
| Operational transparency | 0.0 |
| Developer ergonomics | 45.2 |
| Access clarity | 34.2 |

**Agent readiness 2.5** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
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

**Regulatory alignment 32.4** — Energy & Utilities

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/hydro-one/](https://apis.io/providers/hydro-one/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Hydro One: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/hydro-one/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
