---
name: Onboard a debtor and a payee relationship
description: Look up companies, create a client-debtor relationship and a client-payee relationship, and assign a factor to the payee.
api: openapi/denim-openapi-original.json
operations:
  - AxlePayWeb.Api.V1.CompanyController.index
  - AxlePayWeb.Api.V1.ClientDebtorRelationshipController.create
  - AxlePayWeb.Api.V1.ClientPayeeRelationshipController.create
  - AxlePayWeb.Api.V1.ClientPayeeRelationshipController.update_assign_factor
---

# Onboard a debtor and a payee relationship

Set up the counterparties a freight broker transacts with: the customer being billed
(debtor) and the carrier/vendor being paid (payee), including the payee's assigned factor.

## Authentication
Send your API key in the `x-api-key` header. See `authentication/denim-authentication.yml`.

## Steps
1. **Find the company** — `GET /api/v1/companies` (`CompanyController.index`) with the
   `query` parameter to search Denim's company network before creating a duplicate.
2. **Create the debtor relationship** — `POST /api/v1/debtor-relationships`
   (`ClientDebtorRelationshipController.create`) to link your client to the debtor. Returns `201`.
3. **Create the payee relationship** — `POST /api/v1/payee-relationships`
   (`ClientPayeeRelationshipController.create`) to link your client to the carrier/payee.
4. **Assign a factor** — if the payee is factored, call
   `POST /api/v1/payee-relationships/{client_payee_relationship_id}/update-assign-factor`
   (`ClientPayeeRelationshipController.update_assign_factor`). Look up available factors with
   `GET /api/v1/companies/factors` (`FactoringCompanyController.index`).

## Conventions
- Relationship list endpoints accept structured `filters`, plus `page`/`per_page` pagination.
- No idempotency contract is documented; check with the list endpoints before re-creating.
- See `data-model/denim-data-model.yml` for how relationships link companies, debtors,
  payees, and factors.
