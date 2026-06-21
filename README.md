# Multiplier (multiplier)

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
