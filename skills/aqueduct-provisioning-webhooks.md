---
name: Auto-provision on Aqueduct webhooks
description: Register a webhook endpoint and react to provisioning and invoice events to gate access.
api: openapi/aqueduct-openapi.json
operations: [createwebhook, listwebhooks, getProvisioning]
---

# Auto-provision on Aqueduct webhooks

Use this flow to provision and deactivate user access based on billing events.

## Auth
`https://api.tryaqueduct.com/v1`, header `Authorization: Api-Key {key}`, HTTPS only.

## Steps
1. **createwebhook** — register your HTTPS endpoint with the events you care
   about in `enabledEvents` and a signing `secret`. Common events:
   `provisioning.start`, `provisioning.end`, `invoice.paid`.
2. **listwebhooks** — confirm the endpoint is registered.
3. Handle deliveries — each event POSTs the envelope
   `{ createdAt, type, object }`. On `provisioning.start` grant access; on
   `provisioning.end` revoke it; on `invoice.paid` update entitlement.
4. **getProvisioning** — fetch the full Provisioning object by id when you need
   its `start_time` / `end_time` details.

## Notes
- Verify the shared secret on each delivery before acting.
- Aqueduct events map to the AsyncAPI in `asyncapi/aqueduct-webhooks-asyncapi.yml`.
