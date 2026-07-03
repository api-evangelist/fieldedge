# FieldEdge (fieldedge)

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
