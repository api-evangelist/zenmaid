# ZenMaid (zenmaid)

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
