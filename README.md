# Cloudinary (cloudinary)

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
