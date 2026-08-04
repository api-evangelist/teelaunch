# Teelaunch (teelaunch)

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

Teelaunch is a print-on-demand (POD) platform that lets creators design, produce, and dropship custom products - apparel, drinkware, jewelry, home goods, tech accessories, and more - through connected sales channels like Shopify, Etsy, and BigCommerce. Beyond its storefront apps, Teelaunch publishes a documented public REST API that lets developers and high-volume merchants automate the full POD workflow independent of any storefront app.

**Access model:** The API is public and self-service, but gated behind account verification. Any Teelaunch account holder can generate a Bearer (JWT) API token from **Account → Settings → Developer Settings → Generate Token** (see the [API Token article](https://support.teelaunch.com/portal/en/kb/articles/api-token)). Accounts must be verified before the token functions - verification typically completes within 24 hours (up to 72). There is no separate API fee; you pay the standard per-order production and shipping cost when an order is produced.

- **Base URL:** `https://api.teelaunch.com/api/v1`
- **Authentication:** `Authorization: Bearer <token>` (JWT)
- **Interactive docs:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation) (L5 Swagger UI, OpenAPI 3.0)
- **Machine-readable spec:** [`api-docs.json`](https://api.teelaunch.com/api-docs.json) / Postman collection: [`apiCollection.json`](https://api.teelaunch.com/apiCollection.json)

The endpoints in this catalog are **confirmed real** - transcribed from Teelaunch's own published OpenAPI 3.0 document and Postman collection - not modeled.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/apis.yml)

## Tags

- Print on Demand
- POD
- Ecommerce
- Fulfillment
- Dropshipping
- Orders
- Shipping

## Timestamps

- **Created:** 2026-07-11
- **Modified:** 2026-07-11

## APIs

### Teelaunch Account API

Read the authenticated user's account details, manage account settings, store a billing address, and retrieve payment history.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

### Teelaunch Blank Catalog API

Browse Teelaunch's blank (base) product catalog - list blank categories, list and get individual blanks and their variants, look up per-country shipping cost for a blank variant, and create a product directly from a blank.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

### Teelaunch Products API

List and retrieve the products in a Teelaunch account, update a product, and hold or release the orders tied to a product.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

### Teelaunch Orders API

Submit and manage print-on-demand orders - list and get orders, store a new order, create an order from a variant, and cancel, hold, or release orders to control production.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

### Teelaunch Shipping & Tracking API

Retrieve shipment and tracking information for fulfilled orders - by Teelaunch order ID, by order line-item ID, or by platform order ID - plus per-country shipping cost lookups for blank variants. Teelaunch also posts shipment tracking to a webhook URL configured in Developer Settings.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

### Teelaunch Platforms & Stores API

Work with connected sales-channel platforms (Shopify, Etsy, BigCommerce, and others) and their stores - list platforms and stores, list and get platform products, and link, unlink, ignore, or unignore platform products and their variants.

- **Human URL:** [https://api.teelaunch.com/documentation](https://api.teelaunch.com/documentation)
- **Base URL:** `https://api.teelaunch.com/api/v1`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/teelaunch)
- [Website](https://teelaunch.com)
- [Documentation](https://api.teelaunch.com/documentation)
- [Authentication](https://support.teelaunch.com/portal/en/kb/articles/api-token)
- [Plans](plans/teelaunch-plans-pricing.yml)
- [Rate Limits](rate-limits/teelaunch-rate-limits.yml)
- [Fin Ops](finops/teelaunch-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
