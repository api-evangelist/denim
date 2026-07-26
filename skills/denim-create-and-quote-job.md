---
name: Create and quote a freight job
description: Create a freight load (job) in Denim, get a factoring quote for it, attach a document, and inspect the created job.
api: openapi/denim-openapi-original.json
operations:
  - AxlePayWeb.Api.V1.JobController.get_quote
  - AxlePayWeb.Api.V1.JobController.create
  - Elixir.AxlePayWeb.Api.V1.Job.DocumentController.create
  - AxlePayWeb.Api.V1.JobController.show
---

# Create and quote a freight job

Use the Denim Public API to create a freight load ("job"), get a factoring quote, attach
supporting documents, and read the resulting job record.

## Authentication
All requests require an API key sent in the `x-api-key` request header. Production base URL
is `https://app.denim.com`; staging is `https://staging.denim.com`. See
`authentication/denim-authentication.yml`.

## Steps
1. **Get a quote** — `POST /api/v1/jobs/quote` (`JobController.get_quote`). Submit the load
   details (route stops, shipment items, mode) to receive a factoring quote before committing.
2. **Create the job** — `POST /api/v1/jobs` (`JobController.create`), or the revised
   `POST /api/v2/jobs` (`V2.JobController.create`). Provide the debtor, load route, and shipment
   details. Returns `201` with the created job.
3. **Attach a document** — `POST /api/v1/jobs/{job_id}/documents`
   (`Job.DocumentController.create`) to upload the rate confirmation / BOL / invoice.
4. **Read it back** — `GET /api/v1/jobs/{id}` (`JobController.show`) to confirm status.
5. If corrections are needed before it is finalized, use
   `POST /api/v1/jobs/{job_id}/revert-to-draft` (`JobController.revert_to_draft`).

## Conventions
- List endpoints paginate with `page` and `per_page` (see `conventions/denim-conventions.yml`).
- The spec documents only success responses; handle `401` (bad/missing `x-api-key`) and
  validation errors defensively — no RFC 9457 error envelope is published.
- No idempotency key is supported; do not retry create calls blindly.
