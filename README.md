# Hydro One (hydro-one)

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
