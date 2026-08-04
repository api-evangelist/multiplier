# Multiplier (multiplier)

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

Multiplier (usemultiplier.com) is a global employment platform offering Employer of Record (EOR), Contractor management, and Global Payroll across 150+ countries. Its API surface is integration-oriented - token-authenticated connections used to sync members (employees and contractors), employment contracts, payroll, payments, time off, and invoices between Multiplier and external HRIS systems such as Workday, HiBob, BambooHR, and Personio. Multiplier does not publish an open, self-serve public REST/GraphQL API reference; API access is provisioned per account via Service User tokens. Not to be confused with unrelated companies named "Multiplier".

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/apis.yml)

## Tags

- EOR
- Global Employment
- Payroll
- HR
- Contractors

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## API Availability

Multiplier's API is **not an open, publicly documented self-serve API**. It is an integration surface: customers and partners connect Multiplier to external HRIS, payroll, and identity systems using **Service User tokens** created by an account administrator in Multiplier's Configuration area, passed in an `Authorization` header. Documented partner integrations include Workday (a direct API integration that is an alternative to PECI file exchange), HiBob, BambooHR, and Personio. Because Multiplier does not publish an endpoint-level public API reference, the OpenAPI definition in this repository intentionally carries an empty `paths` object and documents the authentication model and resource scope without fabricating endpoints. The base URLs shown are representative placeholders, not officially published values.

A separate, unrelated product at `docs.multiplierhq.com` also uses the name "Multiplier" and documents its own `request-access` / `get-access-types` endpoints; it is **not** the usemultiplier.com global employment platform profiled here and has been excluded.

## APIs

### Multiplier Members API

Token-authenticated synchronization of Multiplier members - employees and contractors - and their profile, employment, and status data with external HRIS platforms. Exposed through Multiplier's integration program rather than an open public endpoint catalog; the base URL is representative and is not publicly documented.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Members
- Employees
- Contractors
- HRIS

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Multiplier Contracts API

Employment and contractor agreement data - contract generation, terms, and lifecycle status - made available to integrations. Access is provisioned per account; no open public endpoint reference is published.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Contracts
- Employment
- Onboarding

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Multiplier Payroll API

Multi-country payroll data sync - salary, compensation changes, and payroll runs across 120+ currencies. Surfaced to HRIS integrations (for example the Workday API integration, an alternative to PECI file exchange). No open public endpoint reference is published.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Payroll
- Compensation
- Global Payroll

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Multiplier Payments API

Payment and disbursement data for members and contractors. Available to integrations under account-provisioned tokens; no open public endpoint reference is published.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Payments
- Disbursements
- Contractors

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Multiplier Time Off API

Leave requests, balances, and regional holiday data with per-country leave policy rules, plus timesheets. Made available to HRIS integrations; no open public endpoint reference is published.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Time Off
- Leave
- Timesheets

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Multiplier Invoices API

Consolidated invoice and billing data for employment, payroll, and contractor services. Available to integrations under account-provisioned tokens; no open public endpoint reference is published.

- **Human URL:** [https://help.usemultiplier.com/en/collections/8774534-integrations](https://help.usemultiplier.com/en/collections/8774534-integrations)
- **Base URL:** `https://api.usemultiplier.com`

#### Tags

- Invoices
- Billing
- Finance

#### Properties

- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [OpenAPI](openapi/multiplier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/multiplier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/multiplier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/usemultiplier)
- [Website](https://www.usemultiplier.com)
- [Documentation](https://help.usemultiplier.com/en/collections/8774534-integrations)
- [Plans](plans/multiplier-plans-pricing.yml)
- [Rate Limits](rate-limits/multiplier-rate-limits.yml)
- [Fin Ops](finops/multiplier-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
