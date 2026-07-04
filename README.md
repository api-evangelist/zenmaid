# ZenMaid (zenmaid)

ZenMaid is scheduling and business-management software for maid and house cleaning services - booking, calendar/dispatch, automated SMS and email communication, GPS-verified clock-in/out on a cleaner mobile app, online payments and invoicing, payroll, and reporting. **ZenMaid has no public developer API.** There is no self-service developer portal, no published REST/GraphQL API reference, and no OpenAPI specification of its own. The only documented programmatic surface is a Zapier integration - built and maintained by ZenMaid against a private, undocumented backend API - with no API keys, base URL, endpoint reference, payload schema, or SDK published for third-party developers. This repository is documented as a stub because there is no public API to catalog.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/zenmaid/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/zenmaid/refs/heads/main/apis.yml)

## Tags

- Maid Service
- Cleaning Business Software
- Field Service
- Scheduling
- Zapier
- No Public API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

None. ZenMaid does not publish a public API. See [review.yml](review.yml) for the full findings.

## Zapier Integration (not a public API)

ZenMaid's only documented automation surface is its official Zapier app (zapier.com/apps/zenmaid-nWD), which exposes:

**Triggers**

- New Customer Created
- Appointment Booked
- Appointment Cancelled
- Appointment Updated
- Contact Created
- Contact Updated
- One-Time Service Created
- One-Time Service Updated
- Recurring Service Created
- Recurring Service Updated
- Recurring Service Cancelled
- Invoice Created
- Invoice Paid

**Actions**

- Create Appointment
- Create Booking
- Create Cleaner
- Create Customer

Zapier itself notes that payment processing (Square, Venmo, etc.) and transferring cleaning costs are not supported through this integration. These triggers and actions run against ZenMaid's own private backend API, which is not published, versioned, or documented for outside developers - there is no way for a third-party to call it directly outside of Zapier (or Zapier-compatible AI/MCP wrappers such as viaSocket's ZenMaid MCP server, which likewise sits on top of the same Zapier actions rather than a documented ZenMaid API).

## Common Properties

- [Website](https://www.zenmaid.com)
- [LinkedIn](https://www.linkedin.com/company/zenmaid)
- [GitHub Organization](https://github.com/zenmaid)
- [Integrations](https://get.zenmaid.com/zapier)
- [Documentation](https://answers.zenmaid.com/en/collections/39144-integrations)
- [Help Center](https://answers.zenmaid.com)
- [Plans](plans/zenmaid-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
