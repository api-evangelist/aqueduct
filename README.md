# Aqueduct

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

Aqueduct is a fintech billing platform that equips B2B businesses with billing, invoicing, quoting, and accounting for usage-based and metered business models. Developers configure how they collect money as a PriceModel (composed of price functions such as per-unit meters), send billable usage events, and let Aqueduct create invoices and subscriptions, send invoices by email, issue refunds, and auto-provision access via signed webhooks. The REST API lives at api.tryaqueduct.com/v1 with API-key authentication and a documented Idempotency-Key contract. Founded 2020 in Bellevue, WA and backed by Bain Capital Ventures and Conversion Capital, Aqueduct was acquired by Stripe in August 2024; its ReadMe developer portal at docs.tryaqueduct.com remains live.

**Areas:** Company · Fintech · Billing · Invoicing · Metering · Usage-Based · Subscription · Payments

## Aqueduct on APIs.io

Everything profiled for Aqueduct is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/aqueduct/](https://apis.io/providers/aqueduct/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Aqueduct AccountOwner API](https://apis.io/apis/aqueduct/aqueduct-accountowner-api/) — The AccountOwner API from Aqueduct — 3 operation(s) for accountowner.
- [Aqueduct Bill API](https://apis.io/apis/aqueduct/aqueduct-bill-api/) — The Bill API from Aqueduct — 2 operation(s) for bill.
- [Aqueduct Invoice API](https://apis.io/apis/aqueduct/aqueduct-invoice-api/) — The Invoice API from Aqueduct — 6 operation(s) for invoice.
- [Aqueduct PriceModel API](https://apis.io/apis/aqueduct/aqueduct-pricemodel-api/) — The PriceModel API from Aqueduct — 3 operation(s) for pricemodel.
- [Aqueduct ProductPurchases API](https://apis.io/apis/aqueduct/aqueduct-productpurchases-api/) — The ProductPurchases API from Aqueduct — 1 operation(s) for productpurchases.
- [Aqueduct Products API](https://apis.io/apis/aqueduct/aqueduct-products-api/) — The Products API from Aqueduct — 2 operation(s) for products.
- [Aqueduct Provisioning API](https://apis.io/apis/aqueduct/aqueduct-provisioning-api/) — The Provisioning API from Aqueduct — 1 operation(s) for provisioning.
- [Aqueduct Subscriptions API](https://apis.io/apis/aqueduct/aqueduct-subscriptions-api/) — The Subscriptions API from Aqueduct — 2 operation(s) for subscriptions.
- [Aqueduct Webhooks API](https://apis.io/apis/aqueduct/aqueduct-webhooks-api/) — The Webhooks API from Aqueduct — 1 operation(s) for webhooks.
- [Aqueduct Invoice Line Item API](https://apis.io/apis/aqueduct/aqueduct-invoice-line-item-api/) — The Invoice Line Item API from Aqueduct — 1 operation(s) for invoice line item.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Aqueduct Webhooks](https://apis.io/asyncapis/aqueduct/aqueduct-webhooks-asyncapi/)

#### Event channels (1)

Individual events and webhooks the provider emits.

- [{subscriberUrl}](https://apis.io/channels/aqueduct/subscriberurl/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [aqueduct](https://apis.io/servers/aqueduct/aqueduct/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Aqueduct Agentic Access](https://apis.io/agentic-access/aqueduct/aqueduct-agentic-access/)

#### Collections (10)

Postman and Open Collection request collections.

- [Aqueduct API Reference AccountOwner API](https://apis.io/collections/aqueduct/open-aqueduct-accountowner-api/)
- [Aqueduct API Reference AccountOwner Bill API](https://apis.io/collections/aqueduct/open-aqueduct-bill-api/)
- [Aqueduct API Reference AccountOwner Invoice API](https://apis.io/collections/aqueduct/open-aqueduct-invoice-api/)
- [Aqueduct API Reference AccountOwner InvoiceLineItem API](https://apis.io/collections/aqueduct/open-aqueduct-invoicelineitem-api/)
- [Aqueduct API Reference AccountOwner PriceModel API](https://apis.io/collections/aqueduct/open-aqueduct-pricemodel-api/)
- [Aqueduct API Reference AccountOwner ProductPurchases API](https://apis.io/collections/aqueduct/open-aqueduct-productpurchases-api/)
- [Aqueduct API Reference AccountOwner Products API](https://apis.io/collections/aqueduct/open-aqueduct-products-api/)
- [Aqueduct API Reference AccountOwner Provisioning API](https://apis.io/collections/aqueduct/open-aqueduct-provisioning-api/)
- [Aqueduct API Reference AccountOwner Subscriptions API](https://apis.io/collections/aqueduct/open-aqueduct-subscriptions-api/)
- [Aqueduct API Reference AccountOwner Webhooks API](https://apis.io/collections/aqueduct/open-aqueduct-webhooks-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Aqueduct Openapi Overlay](https://apis.io/overlays/aqueduct/aqueduct-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Aqueduct Authentication](https://apis.io/security/aqueduct/aqueduct-authentication/)
- [Aqueduct Domain Security](https://apis.io/security/aqueduct/aqueduct-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.tryaqueduct.com/)
- [Documentation](https://docs.tryaqueduct.com/reference)
- [Getting started](https://docs.tryaqueduct.com/reference/getting-started-with-your-api)
- [API reference](https://docs.tryaqueduct.com/reference)

## API Evangelist rating

**Kin Score 29.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 50.5 |
| Contract governance | 4.5 |
| Operational transparency | 7.9 |
| Developer ergonomics | 32.7 |
| Access clarity | 0.0 |

**Agent readiness 29.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 15.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/aqueduct/](https://apis.io/providers/aqueduct/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Aqueduct: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/aqueduct/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
