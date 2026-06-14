# Cloudinary GraphQL Schema

## Overview

Cloudinary does not currently expose a public GraphQL API. This conceptual schema represents the domain model of Cloudinary's media management and transformation platform, derived from their REST APIs (Upload API, Admin API, Search API, Provisioning API, Permissions API, and Transformation URL API). It is provided to support tooling, federation, and integration design work.

## Source APIs

- **Upload API** — `https://api.cloudinary.com/v1_1` — upload, manage, and transform assets
- **Admin API** — `https://api.cloudinary.com/v1_1` — bulk asset management, folders, metadata, presets, webhooks
- **Search API** — `https://api.cloudinary.com/v1_1` — Lucene-style asset search with visual similarity
- **Provisioning API** — `https://api.cloudinary.com/v1_1/provisioning` — environments, users, groups, API keys
- **Permissions API** — `https://api.cloudinary.com/v1_1` — granular RBAC on assets and folders
- **Transformation URL API** — `https://res.cloudinary.com` — URL-based on-the-fly transformations

## Authentication

All REST endpoints use HTTP Basic Authentication with an API key and secret. Signed upload requests include a HMAC-SHA1 `signature` parameter. Delivery URLs for restricted assets use signed tokens.

## Schema Source

Conceptual — hand-authored from Cloudinary public documentation and REST API surfaces. No introspection was available at `https://api.cloudinary.com/graphql` (404).

## Key Design Decisions

- `Asset` is the central union of `Image`, `Video`, and `RawFile` resource types.
- `TransformationLayer` models a single chained transformation step; `TransformationString` models the full compiled URL segment.
- `StructuredMetadata` and `MetadataField` reflect Cloudinary's typed metadata schema (string, integer, date, enum, set).
- `UploadPreset` captures all upload configuration defaults including eager transformations and access controls.
- `StreamProfile` and `LiveStream` cover adaptive bitrate streaming and live video capabilities.
- `Sprite`, `MultiImage`, and `Archive` represent Cloudinary's batch/composite asset generation features.
- `Permission` and `AccessToken` model RBAC and signed URL delivery controls.

## Types Summary

| Category | Types |
|---|---|
| Core Assets | Asset, Image, Video, RawFile, AssetVersion, ResourceType, DeliveryType |
| Storage & Folders | Folder, StoredURL, FetchedURL, BackupStatus |
| Metadata | Context, StructuredMetadata, MetadataField, Tag |
| Transformations | TransformationLayer, TransformationString, TransformationTemplate, Effect, Adjustment, CropMode, Gravity, Format, Quality, Overlay, Underlay |
| Upload | Upload, UploadPreset, Signature, Timestamp |
| Delivery | Sprite, MultiImage, Archive |
| Streaming | StreamProfile, LiveStream, VideoChapter |
| Access Control | AccessControl, Permission, AccessToken |
| Notifications | Notification, WebhookNotification |
| Operations | BulkResult, RestoreResult |
| Media Library | MediaLibrary |

## Schema File

See `cloudinary-schema.graphql` for the full type definitions.
