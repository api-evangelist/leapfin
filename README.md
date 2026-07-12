# Leapfin (leapfin)

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
