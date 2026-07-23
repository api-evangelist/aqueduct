---
name: Set up usage-based billing on Aqueduct
description: Create a customer and a usage-based price model, send metered usage, and bill it into an invoice.
api: openapi/aqueduct-openapi.json
operations: [createAccountOwner, createPriceModel, sendBillableEvents, bill, getInvoice]
---

# Set up usage-based billing on Aqueduct

Use this flow to stand up a metered business model: charge a customer based on
usage they generate.

## Auth
All requests go to `https://api.tryaqueduct.com/v1` over HTTPS. Send your API key
in the header: `Authorization: Api-Key {key}`.

## Idempotency
Put an `Idempotency-Key: <uuid>` header on every POST so retries never
double-charge. Keys are honored for at least 24 hours. `sendBillableEvents` also
accepts a per-event `idempotencyKey` so batched events are not double-counted.

## Steps
1. **createAccountOwner** — create the customer (the account owner) to be billed.
   Keep the returned id; it is the `customerId` referenced everywhere else.
2. **createPriceModel** — define how much and how often to charge. A price model
   holds one or more price functions (e.g. a `per-unit-meter` function with a
   meter name and rate) and a billing frequency (one-time, monthly, annually).
3. **sendBillableEvents** — report usage as billable events keyed to the meter
   name and the customer. Attach an `idempotencyKey` per event.
4. **bill** — bill the customer against the price model; Aqueduct creates the
   invoice and subscription as needed.
5. **getInvoice** — retrieve the resulting invoice to confirm amounts and status.

## Notes
- List/preview endpoints (`listPriceModels`, `previewPriceModel`) help you verify
  a model before billing against it.
- GET and DELETE are inherently idempotent; no key needed.
