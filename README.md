# ServiceM8 (servicem8)

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
