# Hydro One (hydro-one)

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

Hydro One Limited (TSX: H) is Canada's largest electricity transmission and distribution service provider, transmitting and distributing electricity across Ontario — the province the company describes as "home to 38 per cent of Canada's population." It sits in the regulated wires tier of the value chain: it owns and operates the provincial transmission grid and a rural/regional distribution network, while the Ontario market itself is operated by the IESO and rates are set by the Ontario Energy Board. Its API posture is defined entirely by regulation, not by product. Ontario Regulation 633/21 (Energy Data, under the Electricity Act, 1998) compels Ontario electricity and natural gas distributors to implement Green Button Download My Data (DMD) and Connect My Data (CMD) and to have those implementations certified by the Green Button Alliance. Hydro One publishes DMD as an authenticated XML export inside My Account, runs a live Green Button CMD OAuth 2.0 authorization surface, and operates a published third-party vendor onboarding form and terms — but the CMD resource base URI, client credentials, and test accounts are issued privately during onboarding and are not published anywhere. There is no developer subdomain, no OpenAPI or Swagger definition, and no self-serve signup.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/hydro-one/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/hydro-one/refs/heads/main/apis.yml)

## Tags

- Energy
- Canada
- Utilities
- Electricity
- Grid
- Smart Metering
- Green Button
- Energy Data
- Transmission
- Distribution

## Timestamps

- **Created:** 2026-07-27
- **Modified:** 2026-07-27

## APIs

### Hydro One Green Button Connect My Data (CMD)

Hydro One's Green Button Connect My Data implementation, mandated by Ontario Regulation 633/21. A registered third-party vendor obtains an OAuth 2.0 authorization code after the customer authenticates with Hydro One and consents, then retrieves that customer's electricity usage and billing data as NAESB ESPI XML. Hydro One does not publish the CMD resource base URI, an OpenAPI definition, or any endpoint reference — Client ID, Client Secret, test accounts, and URI(s) are issued privately during vendor onboarding, followed by a 90-day connectivity test and an exchange of RSA 2048-bit certificates over TLS.

- **Human URL:** [https://www.hydroone.com/saving-money-and-energy/green-button/third-party-apps](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-apps)
- **Base URL:** not published — issued privately during vendor onboarding

#### Tags

- Green Button
- Connect My Data
- ESPI
- Energy Data
- OAuth2
- Consumer Data

#### Properties

- [Documentation](https://www.hydroone.com/saving-money-and-energy/green-button)
- [Documentation](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-apps)
- [Terms of Service](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions)
- [Sign Up](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-onboarding-form)
- [Authentication](https://www.hydroone.com/green-button-cmd-home)
- [Regulation](https://www.ontario.ca/laws/regulation/210633)
- [Standard](https://www.greenbuttonalliance.org/)
- [Regulator](https://www.oeb.ca/consumer-information-and-protection/green-button)

## Mandate

- **Regime:** `green-button-ontario` — O. Reg. 633/21 (Energy Data), Electricity Act, 1998, s. 25.35.8
- **Status:** `live-implemented` — verified from a live CMD authorization surface carrying NAESB ESPI function-block scope syntax, plus a published third-party onboarding form and terms describing credential issuance and 90-day connectivity testing. Not recorded from a compliance claim.
- **Data standard:** Green Button DMD and CMD over NAESB REQ.21 ESPI (Ontario certification tied to v3.3); ESPI XML payloads
- **Consumer data API:** yes — consent-gated, accreditation-free, utility-approved
- **Open market data:** no — Hydro One publishes no open grid or system data API; Ontario market data belongs to the IESO
- **Access gate:** `application-approval` — accept terms, register on the HONI third-party portal, receive Client ID / Client Secret / test accounts / URI(s), pass connectivity testing within 90 days, exchange RSA 2048-bit certificates over TLS
- **Auth model:** OAuth 2.0 authorization code with ESPI `FB=` scopes; no OpenID Connect discovery document is served
- **Home market:** Canada

## Common Properties

- [Website](https://www.hydroone.com/)
- [About](https://www.hydroone.com/about)
- [Documentation](https://www.hydroone.com/saving-money-and-energy/green-button)
- [Terms of Service](https://www.hydroone.com/saving-money-and-energy/green-button/third-party-terms-and-conditions)
- [LinkedIn](https://www.linkedin.com/company/hydro-one)
- [Regulator](https://www.oeb.ca/consumer-information-and-protection/green-button)

## Maintainers

- Kin Lane — kin@apievangelist.com
