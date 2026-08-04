# Cloudinary (cloudinary)

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

Cloudinary is a cloud-based service that provides comprehensive solutions for managing digital media assets, including images and videos, for websites and mobile applications. The platform exposes REST APIs for uploading and transforming media, administering assets and product environments, provisioning users and accounts, and configuring granular permissions. APIs use Basic Authentication with API key and secret over HTTPS.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Asset Management
- Digital Asset Management
- Image Processing
- Image Transformation
- Media
- SaaS
- Video Processing

## Timestamps

- **Created:** 2024-11-13
- **Modified:** 2026-05-30

## APIs

### Cloudinary Upload API

The Upload API exposes methods for uploading and managing assets, including advanced upload options, CRUD operations on assets, metadata management, eager and on-the-fly transformations, signed and unsigned uploads, and creation of new asset variants from existing originals. Endpoints are versioned under /v1_1/:cloud_name/:resource_type and use HTTP Basic Auth with API key and secret.

- **Human URL:** [https://cloudinary.com/documentation/image_upload_api_reference](https://cloudinary.com/documentation/image_upload_api_reference)
- **Base URL:** `https://api.cloudinary.com/v1_1`

#### Tags

- Asset Upload
- Image Processing
- Media
- Transformation

#### Properties

- [Documentation](https://cloudinary.com/documentation/image_upload_api_reference)
- [Getting Started](https://cloudinary.com/documentation/upload_images)
- [OpenAPI](openapi/cloudinary-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Admin API

The Admin API supports bulk asset management (search, retrieval, update, delete, restore), and CRUD management of folders, metadata fields, metadata rules, upload presets, transformations, streaming profiles, webhooks, mappings and product environment configuration. Authentication uses HTTP Basic Auth with API key and secret. EU and AP regional endpoints are available for enterprise customers (api-eu.cloudinary.com, api-ap.cloudinary.com).

- **Human URL:** [https://cloudinary.com/documentation/admin_api](https://cloudinary.com/documentation/admin_api)
- **Base URL:** `https://api.cloudinary.com/v1_1`

#### Tags

- Administration
- Asset Management
- Folders
- Metadata
- Webhooks

#### Properties

- [Documentation](https://cloudinary.com/documentation/admin_api)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Search API

The Search API exposes Lucene-style query expressions across asset metadata, tags, contextual metadata, structured metadata, and AI-derived tags. Supports sorting, aggregation, pagination via cursors, and saved searches. Visual search and similarity search use perceptual hashes and embeddings to find visually similar assets.

- **Human URL:** [https://cloudinary.com/documentation/search_api](https://cloudinary.com/documentation/search_api)
- **Base URL:** `https://api.cloudinary.com/v1_1`

#### Tags

- Asset Discovery
- Search
- Visual Search

#### Properties

- [Documentation](https://cloudinary.com/documentation/search_api)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Provisioning API

The Provisioning API enables enterprise account-level management of product environments (sub-accounts), users, user groups, and API keys. Authentication uses provisioning API key and secret. Useful for onboarding teams, rotating credentials, and automating environment lifecycle in multi-tenant deployments.

- **Human URL:** [https://cloudinary.com/documentation/provisioning_api](https://cloudinary.com/documentation/provisioning_api)
- **Base URL:** `https://api.cloudinary.com/v1_1/provisioning`

#### Tags

- Account Management
- API Keys
- Provisioning
- Users

#### Properties

- [Documentation](https://cloudinary.com/documentation/provisioning_api)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Permissions API

The Permissions API assigns granular permissions to principals (users, groups, API keys) by roles or directly. Supports folder-scoped, asset- scoped, and product-environment-scoped permission grants and listing.

- **Human URL:** [https://cloudinary.com/documentation/permissions_api](https://cloudinary.com/documentation/permissions_api)
- **Base URL:** `https://api.cloudinary.com/v1_1`

#### Tags

- Access Control
- Permissions
- RBAC
- Roles

#### Properties

- [Documentation](https://cloudinary.com/documentation/permissions_api)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Transformation URL API

The Transformation URL API delivers and transforms images and videos by composing parameters into the delivery URL path (/{cloud_name}/{resource_type}/{type}/{transformations}/{public_id}). Supports resizing, cropping, color and effect transformations, format conversion, watermarks, overlays, AI-driven content-aware operations, and conditional transformations.

- **Human URL:** [https://cloudinary.com/documentation/transformation_reference](https://cloudinary.com/documentation/transformation_reference)
- **Base URL:** `https://res.cloudinary.com`

#### Tags

- Delivery
- Image Transformation
- URL API
- Video Transformation

#### Properties

- [Documentation](https://cloudinary.com/documentation/transformation_reference)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cloudinary Notifications and Webhooks

Cloudinary fires HTTP webhook notifications for upload completion, eager transformation completion, AI moderation outcomes, asset deletion, and backup events. Notifications include signatures for verification and can target multiple endpoints per product environment.

- **Human URL:** [https://cloudinary.com/documentation/notifications](https://cloudinary.com/documentation/notifications)

#### Tags

- Events
- Notifications
- Webhooks

#### Properties

- [Documentation](https://cloudinary.com/documentation/notifications)
- [AsyncAPI](asyncapi/cloudinary-notifications-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/cloudinary.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cloudinary.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/cloudinary)
- [Website](https://cloudinary.com/)
- [Portal](https://console.cloudinary.com/)
- [Documentation](https://cloudinary.com/documentation)
- [Sign Up](https://cloudinary.com/users/register_free)
- [Pricing](https://cloudinary.com/pricing)
- [Status Page](https://status.cloudinary.com/)
- [Git Hub](https://github.com/cloudinary)
- [Terms of Service](https://cloudinary.com/tos)
- [Privacy](https://cloudinary.com/privacy)
- [Features](undefined)
- [Integrations](https://cloudinary.com/integrations)
- [L L Ms Txt](https://cloudinary.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
