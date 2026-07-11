# Teelaunch (teelaunch)

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
