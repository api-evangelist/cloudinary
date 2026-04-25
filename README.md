# Cloudinary (cloudinary)

Cloudinary is a cloud-based service that provides comprehensive solutions for managing digital media assets, including images and videos, for websites and mobile applications. The platform exposes REST APIs for uploading and transforming media, administering assets and product environments, provisioning users and accounts, and configuring granular permissions. APIs use Basic Authentication with API key and secret over HTTPS.

**APIs.json:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party
- **x-type:** company

## Tags

Asset Management, Digital Asset Management, Image Processing, Image Transformation, Media, SaaS, Video Processing

## Timestamps

- **Created:** 2024-11-13
- **Modified:** 2026-04-23

## APIs

### Cloudinary Upload API
Upload and manage assets including advanced upload options, CRUD operations, metadata management, eager and on-the-fly transformations, signed and unsigned uploads, and creating new asset variants from existing originals.

- Base URL: `https://api.cloudinary.com/v1_1`
- [Documentation](https://cloudinary.com/documentation/image_upload_api_reference)

### Cloudinary Admin API
Bulk asset management (search, retrieval, update, delete, restore) and CRUD on folders, metadata fields, metadata rules, upload presets, transformations, streaming profiles, webhooks, and product environment configuration. EU and AP regional endpoints are available for enterprise customers.

- Base URL: `https://api.cloudinary.com/v1_1`
- [Documentation](https://cloudinary.com/documentation/admin_api)

### Cloudinary Search API
Lucene-style queries across asset metadata, tags, contextual metadata, structured metadata, and AI-derived tags. Supports sorting, aggregation, cursor pagination, and visual similarity search.

- [Documentation](https://cloudinary.com/documentation/search_api)

### Cloudinary Provisioning API
Enterprise-account management of product environments (sub-accounts), users, user groups, and API keys. Authentication uses provisioning API key and secret.

- Base URL: `https://api.cloudinary.com/v1_1/provisioning`
- [Documentation](https://cloudinary.com/documentation/provisioning_api)

### Cloudinary Permissions API
Assign granular permissions to principals (users, groups, API keys) by roles or directly. Supports folder-, asset-, and environment-scoped permission grants.

- [Documentation](https://cloudinary.com/documentation/permissions_api)

### Cloudinary Transformation URL API
Deliver and transform media via URL parameters: resizing, cropping, color/effect transformations, format conversion, watermarks, overlays, AI-driven content-aware operations, and conditional transformations.

- Base URL: `https://res.cloudinary.com`
- [Documentation](https://cloudinary.com/documentation/transformation_reference)

### Cloudinary Notifications and Webhooks
HTTP webhook notifications for upload completion, eager transformation completion, AI moderation outcomes, asset deletion, and backup events. Includes signatures for verification.

- [Documentation](https://cloudinary.com/documentation/notifications)

## Common Properties

- [Website](https://cloudinary.com/)
- [Portal](https://console.cloudinary.com/)
- [Documentation](https://cloudinary.com/documentation)
- [SignUp](https://cloudinary.com/users/register_free)
- [Pricing](https://cloudinary.com/pricing)
- [Status](https://status.cloudinary.com/)
- [GitHub](https://github.com/cloudinary)

## Maintainers

- **FN:** Kin Lane
- **Email:** kin@apievangelist.com
