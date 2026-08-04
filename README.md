# Leapfin (leapfin)

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

Leapfin is an AI-powered financial data platform for **record-to-report** and **automated revenue recognition**. It ingests transactional data from billing systems, payment processors, and data warehouses, standardizes it into a unified **Financial Records** schema, applies templated GAAP, SOX, IFRS, and **ASC 606** revenue rules, and produces audit-ready **journal entries** and revenue **reports** that post to ERPs such as NetSuite. Customers include Canva, Reddit, SeatGeek, and Flexport.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/leapfin/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/leapfin/refs/heads/main/apis.yml)

## Access Model (Read This First)

Leapfin is **enterprise SaaS**. It exposes one documented programmatic surface, the **Leap Connect API** (released March 22, 2024), used to **ingest** transactional data into the platform - typically pushed over HTTPS in a nightly batch. The full developer reference lives on a ReadMe-style portal at [docs.leapfin.com](https://docs.leapfin.com/) that is **bot-blocked (HTTP 403) and partner/login-gated**, so exact endpoint paths, base URL, and authentication could not be reproduced for this catalog entry.

Because of that gating:

- The APIs listed below are **logical APIs modeled** from Leapfin's public product and help-center material. **No endpoint paths were fabricated** and no base URLs are asserted.
- Third-party trackers ([apitracker.io](https://apitracker.io/a/leapfin)) report that an OpenAPI/Swagger spec plus Postman and Insomnia collections exist (ReadMe auto-generates these), but the underlying specification is not retrievable without authentication, so **no `openapi/` or `collections/` files were created**.
- No `rate-limits/` or `finops/` files were created - Leapfin does not publish that data.
- Pricing is **contact-sales / enterprise only** (see [plans](plans/leapfin-plans-pricing.yml)); there is no public free or self-service tier.

## Tags

- Revenue Recognition
- ASC 606
- Financial Automation
- Accounting
- Revenue Accounting
- Record to Report
- Journal Entries
- Data Ingestion

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

> All APIs below are marked **endpointsModeled** - derived from public product/help pages, not from the gated endpoint reference. See [review.yml](review.yml) for the full access-model assessment.

### Leapfin Leap Connect Data Ingestion API

Leapfin's documented programmatic ingestion surface. Developers push transactional data - typically nightly batch - into Leapfin's ingestion services, where it is transformed into the unified Financial Records schema for downstream revenue recognition and journal-entry generation.

- **Human URL:** [https://docs.leapfin.com/docs/custom-integrations](https://docs.leapfin.com/docs/custom-integrations)
- Documentation, API Reference, and Help Center links in `apis.yml`.

### Leapfin Financial Records API

Modeled surface for the unified accounting-ready schema that ingested billing, payment, and warehouse data is normalized into, with links tracing every transaction across the order-to-cash process.

### Leapfin Revenue Recognition API

Modeled surface for automated revenue recognition - templated ASC 606 and IFRS revenue rules applied across large volumes of Financial Records for accounting consistency and compliance.

### Leapfin Journal Entries API

Modeled surface for balanced, GL-ready journal entries produced for each revenue recognition activity and delivered to ERPs such as NetSuite.

### Leapfin Reports API

Modeled surface for consolidated revenue reports and month-over-month views drillable to the individual transaction, plus natural-language exploration via the Luca AI agent.

### Leapfin Webhooks API

Modeled surface for event notifications referenced on Leapfin's developer portal and third-party trackers. Exact event types and payloads are behind the gated portal.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/leapfin)
- [Website](https://www.leapfin.com)
- [Documentation](https://docs.leapfin.com/)
- [Help Center](https://help.leapfin.com/)
- [Plans](plans/leapfin-plans-pricing.yml)
- [Blog](https://www.leapfin.com/blog)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
