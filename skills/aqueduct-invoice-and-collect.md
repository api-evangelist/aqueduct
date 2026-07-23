---
name: Issue and collect an invoice on Aqueduct
description: Create an invoice, add line items, send it to the customer, and handle refunds or voids.
api: openapi/aqueduct-openapi.json
operations: [createInvoice, createInvoiceLineItem, sendInvoice, getInvoice, refundInvoice, voidInvoice]
---

# Issue and collect an invoice on Aqueduct

Use this flow to bill a customer directly with an ad-hoc invoice.

## Auth
`https://api.tryaqueduct.com/v1`, header `Authorization: Api-Key {key}`, HTTPS only.
Put an `Idempotency-Key: <uuid>` header on every POST.

## Steps
1. **createInvoice** — create an invoice for a `customerId` in a supported
   currency (USD or CAD). You may include line items inline or add them next.
2. **createInvoiceLineItem** — add each charge line (description + amount) to the
   invoice by `invoiceId`.
3. **sendInvoice** — email the invoice to the customer. All parameters are
   overrides; defaults come from the organization's email settings.
4. **getInvoice** — poll the invoice to observe its status (e.g. paid). An
   `invoice.paid` webhook fires when it is paid.

## Corrections
- **refundInvoice** — refund an invoice when possible (e.g. credit-card
  payments). Returns `400` if a refund is not possible.
- **voidInvoice** — mark an invoice as void when it should not be collected.

## Notes
- Generate a hosted customer view with `createCustomerPortalLink` for the account
  owner.
