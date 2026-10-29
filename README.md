# Denim

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

Denim (denim.com, formerly Axle Payments) is an all-in-one financial and back-office platform for freight brokers, trucking companies, and 3PLs. It provides freight factoring, invoicing, collections, carrier payments, and a fuel card, automating the broker back office and syncing two ways with transportation management systems. The Denim Public API (OpenAPI 3.0) exposes freight loads (jobs), debtors, payees, companies, factoring companies, and transactions, secured with an x-api-key header, so partners can create and quote jobs, onboard debtor/payee relationships, and reconcile transactions programmatically. Added to the API Evangelist network as a portfolio-company lead and enriched from the provider's public developer surface.

**Areas:** Company · Freight · Factoring · Payments · Logistics · Trucking · Fintech · Back Office

## Denim on APIs.io

Everything profiled for Denim is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/denim/](https://apis.io/providers/denim/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Denim Companies API](https://apis.io/apis/denim/denim-companies-api/) — A company in our system includes Payees, Debtors, and Factoring companies. Companies records are available globally in our ecosystem and shared by other…
- [Denim Debtors API](https://apis.io/apis/denim/denim-debtors-api/) — A debtor is your customer or shipper. They are the entity that will be paying the invoices. Debtors are a type of Company in our ecosystem and are…
- [Denim Jobs API](https://apis.io/apis/denim/denim-jobs-api/) — A job is a collection of obligations (payables, receivables, and fees) associated with an invoice or purchase order.
- [Denim Jobs V2 API](https://apis.io/apis/denim/denim-jobs-v2-api/) — Version 2. A job is a collection of obligations (payables, receivables, and fees) associated with an invoice or purchase order.
- [Denim Payees API](https://apis.io/apis/denim/denim-payees-api/) — A payee is your contractor or carrier. They are the entity that needs to be paid for services. Payees are a type of Company in our ecosystem and are…
- [Denim Transactions API](https://apis.io/apis/denim/denim-transactions-api/) — Transactions are payments incoming, outgoing, netting, and adjustments. Transactions are are generally applied towards obligations.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [denim](https://apis.io/servers/denim/denim/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Denim Agentic Access](https://apis.io/agentic-access/denim/denim-agentic-access/)

#### Collections (6)

Postman and Open Collection request collections.

- [Denim Public API Reference Documentation Companies API](https://apis.io/collections/denim/open-denim-companies-api/)
- [Denim Public API Reference Documentation Companies Debtors API](https://apis.io/collections/denim/open-denim-debtors-api/)
- [Denim Public API Reference Documentation Companies Jobs API](https://apis.io/collections/denim/open-denim-jobs-api/)
- [Denim Public API Reference Documentation Companies Jobs V2 API](https://apis.io/collections/denim/open-denim-jobs-v2-api/)
- [Denim Public API Reference Documentation Companies Payees API](https://apis.io/collections/denim/open-denim-payees-api/)
- [Denim Public API Reference Documentation Companies Transactions API](https://apis.io/collections/denim/open-denim-transactions-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Denim Openapi Overlay](https://apis.io/overlays/denim/denim-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Denim Authentication](https://apis.io/security/denim/denim-authentication/)
- [Denim Domain Security](https://apis.io/security/denim/denim-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://denim.com/)
- [Documentation](https://app.denim.com/api/v1/documentation)
- [Getting started](https://www.denim.com/denim-api-documents)
- [API reference](https://app.denim.com/api/v1/documentation)
- [Pricing](https://www.denim.com/pricing)
- [Sign up](https://info.denim.com/freightfactoring)
- [Support](https://help.denim.com/hc/en-us)
- [Blog](https://www.denim.com/blog)
- [Terms of service](https://www.denim.com/terms-conditions)
- [Privacy policy](https://www.denim.com/privacy-policy)
- [Status](https://status.denim.com)

## API Evangelist rating

**Kin Score 44.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 52.9 |
| Contract governance | 4.5 |
| Operational transparency | 7.9 |
| Developer ergonomics | 66.1 |
| Access clarity | 44.7 |

**Agent readiness 25.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 22.3** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/denim/](https://apis.io/providers/denim/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Denim: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/denim/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
