# FieldEdge (fieldedge)

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

FieldEdge is field service management (FSM) software for HVAC, plumbing, electrical, and other home- and commercial-services contractors, owned by Xplor Technologies and branded "FieldEdge by Xplor" (formerly dESCO). It provides customer management, dispatching and scheduling, work orders, a technician mobile app, a flat-rate pricebook, service agreements, invoicing and payments, and a QuickBooks accounting sync.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fieldedge/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fieldedge/refs/heads/main/apis.yml)

## API Access Model — Partner-Gated

FieldEdge operates a **real but partner-gated** API. It is delivered through an Azure API Management developer portal at [docs.api.fieldedge.com](https://docs.api.fieldedge.com) ("Providing API access to our integrated partners"). The portal is public to browse and offers sign-up, but the actual **API products, operations, keys, and any OpenAPI definition sit behind the portal sign-in and partner approval** — this is not an openly self-serve public developer API. FieldEdge markets a partner-based integration model with 40+ integration partners and directs prospective integrators to its partners/sales team.

Because the authoritative reference is gated, the logical APIs documented in `apis.yml` are **honestly modeled** (flagged `endpointsModeled: true`) from FieldEdge's documented product modules and its integration surface. No full OpenAPI surface has been fabricated; endpoint paths are inferred, not copied from a published public reference.

## Tags

- Field Service Management
- FSM
- HVAC
- Plumbing
- Electrical
- Home Services
- Dispatch
- Work Orders
- Contractors
- Xplor

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs (modeled)

### FieldEdge Customers API

Manage customers, their service locations, and installed equipment records (make, model, age, and service history). Modeled from the documented Customers & Locations module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

### FieldEdge Work Orders API

Create and track work orders (service calls / jobs) through their lifecycle, including status transitions, notes, attachments (photos), and technician signatures captured in the mobile app. Modeled from the documented Work Orders & Mobile module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

### FieldEdge Dispatch & Scheduling API

Read and manage appointments on the dispatch board — assigning jobs to technicians and viewing scheduled work across technicians and time windows. Modeled from the documented Dispatch/Scheduling module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

### FieldEdge Invoices & Payments API

Generate and retrieve invoices from completed work and record payments, feeding the QuickBooks accounting sync. Modeled from the documented Invoices/Payments module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

### FieldEdge Service Agreements API

Manage recurring service agreements (maintenance plans) tied to customers and equipment, including covered visits and renewal tracking. Modeled from the documented Service Agreements module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

### FieldEdge Pricebook API

Read the flat-rate pricebook of services, parts, and materials used to build quotes and invoices in the field. Modeled from the documented Pricebook module.

- **Human URL:** [https://docs.api.fieldedge.com](https://docs.api.fieldedge.com)
- **Base URL (modeled):** `https://api.fieldedge.com`

## Pricing

FieldEdge is sold as a **per-user monthly subscription** (month-to-month, no long-term contract) for the software product — indicatively ~$100/office user and ~$125/technician per month, with an approximate ~$225/month starting point (1 office user + 1 technician), plus one-time setup/implementation. API access itself is partner-gated and does not carry a separately published, self-serve price. See [plans/fieldedge-plans-pricing.yml](plans/fieldedge-plans-pricing.yml) and [fieldedge.com/pricing](https://fieldedge.com/pricing/).

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/fieldedge)
- [Website](https://fieldedge.com)
- [Documentation (Developer Portal)](https://docs.api.fieldedge.com)
- [Pricing](https://fieldedge.com/pricing/)
- [Plans](plans/fieldedge-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
