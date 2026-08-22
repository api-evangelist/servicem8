# ServiceM8 (servicem8)

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

ServiceM8 is field service and job management software for trade and home-service businesses - electricians, plumbers, HVAC technicians, cleaners, landscapers, and similar contractors. It manages the full job lifecycle from lead and quote through scheduling, dispatch, on-site work, materials, invoicing, and payment. ServiceM8 publishes a documented REST API - plain JSON over HTTP using GET, POST, and DELETE - at `https://api.servicem8.com/api_1.0`, exposing its core objects as individual `.json` endpoints. Private integrations authenticate with an API key (`X-API-Key` header); public add-ons authenticate with OAuth 2.0. Object and event webhook subscriptions push change notifications to a callback URL.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/apis.yml)

## Tags

- Field Service
- Job Management
- Trades
- Scheduling
- Dispatch
- Invoicing
- Home Services

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### ServiceM8 Jobs API

Create, list, retrieve, update, and delete jobs - the central ServiceM8 record covering a piece of work from lead and quote through scheduling, completion, invoicing, and payment.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Job Activities API

Manage job activities - the scheduled bookings and recorded time entries attached to a job, tying a staff member to a job with start and end times.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Clients (Companies) API

Manage clients (called Company in the API) and their company contacts - the customers ServiceM8 does work for.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Job Contacts API

Manage job contacts - the people attached to a specific job in roles such as job contact, billing contact, property owner, or property manager.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Staff API

Manage staff members - the technicians, office users, and field workers referenced by job activities and allocations.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Materials API

Manage the materials catalog and job materials - reusable priced inventory items and the line items added to a specific job's quote or invoice.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Attachments API

Manage attachments - files linked to jobs and other objects, including photos, quotes, invoices, work orders, and signed documents, with binary upload and download.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Queues API

Manage queues - the custom workflow stages a job moves through, used to organise jobs on the dispatch board.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Vendors API

Retrieve and list vendors - the ServiceM8 account records that own the data an integration operates against.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Badges API

Manage badges - the coloured labels used to tag and categorise jobs and clients for filtering and reporting.

- **Human URL:** [https://developer.servicem8.com/docs/rest-overview](https://developer.servicem8.com/docs/rest-overview)
- **Base URL:** `https://api.servicem8.com/api_1.0`

### ServiceM8 Webhooks API

Create and manage object and event webhook subscriptions. When a subscribed field changes, ServiceM8 POSTs the object type, changed fields, uuid, and a resource_url to your callback URL.

- **Human URL:** [https://developer.servicem8.com/docs/webhooks-overview](https://developer.servicem8.com/docs/webhooks-overview)
- **Base URL:** `https://api.servicem8.com`

## Authentication

- **API Key (private apps):** send your key in the `X-API-Key` header.
- **OAuth 2.0 (public add-ons):** authorize at `https://go.servicem8.com/oauth/authorize`, exchange the code at `https://go.servicem8.com/oauth/access_token`; access tokens last 3600 seconds and are refreshable.

## Rate Limits

- 180 requests per minute and 20,000 requests per day, per application per connected account. Exceeding either returns HTTP 429 with the body `Number of allowed API requests per minute exceeded`. Prefer webhooks over polling.

## Common Properties

- [GitHub Organization](https://github.com/servicem8)
- [LinkedIn](https://www.linkedin.com/company/servicem8)
- [Website](https://www.servicem8.com)
- [Documentation](https://developer.servicem8.com/docs)
- [Plans](plans/servicem8-plans-pricing.yml)
- [Rate Limits](rate-limits/servicem8-rate-limits.yml)
- [Fin Ops](finops/servicem8-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
