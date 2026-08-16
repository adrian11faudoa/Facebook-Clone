Using the approved Project 4 — Enterprise Facebook-Style Social Platform Architecture Prompt — Volume 1, Architecture Prompt — Volume 2, and the Master Prompt above.

Begin Backend implementation ONLY.

Do NOT implement frontend, mobile, or infrastructure unless a minimal backend configuration file is required for the backend to run.

Do NOT redesign the approved architecture.

Do NOT redesign service boundaries, database ownership, API contracts, event contracts, authentication architecture, authorization architecture, privacy architecture, or infrastructure architecture.

Assume the Architecture Volumes are the authoritative source of truth.

If an architectural inconsistency makes implementation impossible or unsafe:

1. Identify the inconsistency.
2. Explain the impact.
3. Propose the smallest compatible correction.
4. Do not silently redesign the platform.

────────────────────────────────────────

MISSION

Implement the complete production-ready backend for the Enterprise Facebook-Style Social Platform.

The backend must support:

• Identity

• Authentication

• Authorization

• Users

• Profiles

• Social Graph

• Friendships

• Followers

• Posts

• Media

• Comments

• Reactions

• Sharing

• News Feed

• Recommendations

• Groups

• Communities

• Pages

• Creators

• Businesses

• Events

• Messaging

• Presence

• Notifications

• Search

• Marketplace

• Commerce

• Advertising

• Payment Integration Boundaries

• Analytics

• Moderation

• Trust & Safety

• Spam Detection

• Fraud Detection

• Feature Flags

• Audit Logging

• Developer Platform

• AI Platform Gateway

Implement the backend incrementally according to the Master Prompt milestone strategy.

Each milestone must contain approximately 20–40 files and must leave the generated backend in a consistent, compilable state.

────────────────────────────────────────

BACKEND TECHNOLOGY STACK

Use:

• Node.js

• NestJS

• TypeScript

• PostgreSQL

• Prisma ORM

• Redis

• Kafka or Redpanda

• BullMQ

• Socket.IO

• Elasticsearch or OpenSearch

• AWS S3-compatible object storage

• FFmpeg

• Sharp

• OpenTelemetry

Use strict TypeScript.

Use the architecture-approved monorepo structure.

────────────────────────────────────────

IMPLEMENTATION PRINCIPLES

Strictly apply:

• Clean Architecture

• Domain-Driven Design

• SOLID principles

• Repository Pattern

• Service Layer Pattern

• Dependency Injection

• Feature-first organization

• Explicit domain boundaries

• Database ownership

• Event-driven communication where appropriate

• CQRS only where approved

• Backward compatibility

• Idempotency

• Retry safety

• Graceful failure handling

Do not create unnecessary abstractions.

Do not introduce microservice communication where a local domain interaction is explicitly sufficient.

────────────────────────────────────────

MONOREPO IMPLEMENTATION

Implement the approved monorepo structure.

Maintain clear separation between:

apps/

services/

packages/

infrastructure/

docs/

scripts/

testing/

Create shared packages only when they represent genuinely shared contracts or infrastructure.

Do not place domain business logic into generic shared packages.

────────────────────────────────────────

CORE SHARED BACKEND PACKAGES

Generate and maintain shared backend packages for appropriate concerns including:

• Configuration

• Environment validation

• Structured logging

• Error handling

• HTTP contracts

• Event contracts

• Authentication utilities

• Authorization utilities

• Database utilities

• Redis utilities

• Kafka utilities

• Queue utilities

• Observability

• Validation

• Pagination

• API response models

• Feature flag clients

• Audit utilities

• Testing utilities

All shared packages must have clear ownership and dependency boundaries.

────────────────────────────────────────

CONFIGURATION MANAGEMENT

Implement centralized configuration management.

Support:

• Local development

• Development

• Staging

• Production

Validate all required configuration during startup.

Support typed configuration for:

• Application settings

• Database connections

• Redis

• Kafka or Redpanda

• Elasticsearch or OpenSearch

• Object storage

• Authentication

• OAuth providers

• Email providers

• Notification providers

• Feature flags

• Analytics

• AI providers

• Observability

Never expose secrets through logs or API responses.

────────────────────────────────────────

ERROR HANDLING

Implement a consistent error architecture.

Support:

• Domain errors

• Validation errors

• Authentication errors

• Authorization errors

• Not found errors

• Conflict errors

• Rate-limit errors

• Dependency failures

• Retryable failures

• Non-retryable failures

• Infrastructure errors

Use centralized NestJS exception handling.

Every API error must have a consistent structure.

Do not leak:

• Internal stack traces

• SQL errors

• Secrets

• Internal service topology

• Sensitive user information

────────────────────────────────────────

OBSERVABILITY

Instrument all backend services with OpenTelemetry.

Support:

• Distributed tracing

• Trace propagation

• Request correlation

• Kafka propagation

• Queue propagation

• Structured logs

• Metrics

• Error reporting

Generate consistent telemetry for:

• HTTP requests

• Service calls

• Database operations

• Redis operations

• Kafka producers

• Kafka consumers

• Queue jobs

• WebSocket connections

• Media processing

────────────────────────────────────────

AUTHENTICATION SERVICE

Implement:

• Registration

• Login

• Logout

• Email verification

• Phone verification architecture where approved

• Password hashing

• Password reset

• OAuth

• Refresh tokens

• Access tokens

• Refresh token rotation

• Session management

• Multi-device sessions

• Device registration

• Device management

• Session revocation

• Suspicious login detection hooks

• Multi-factor authentication

• Authenticator application support

• Recovery codes

• Passkey architecture where supported

• Account recovery

• Security notifications

Implement:

• Rate limiting

• Brute-force protection

• Credential stuffing protections

• Secure password policies

• Secure session lifecycle

Never store raw passwords.

Never expose authentication secrets.

────────────────────────────────────────

AUTHORIZATION SERVICE

Implement the approved authorization architecture.

Support:

• RBAC

• Resource-level permissions

• Relationship-aware authorization

• Group permissions

• Community permissions

• Page permissions

• Business permissions

• Marketplace permissions

• Advertising permissions

• Administrative permissions

• Moderation permissions

• Service-to-service authorization

Implement authorization checks server-side.

Do not rely on frontend permission enforcement.

────────────────────────────────────────

IDENTITY, USER, AND PROFILE SERVICES

Implement:

Identity:

• Account identity

• User lifecycle

• Verification state

• Account deletion workflows

• Account recovery boundaries

Users:

• User records

• Account types

• Status

• Privacy state

Profiles:

• Usernames

• Display names

• Bios

• Profile photos

• Cover photos

• Websites

• Professional information

• Profile visibility

• Verification state

• Profile customization

Implement privacy-aware profile retrieval.

────────────────────────────────────────

SOCIAL GRAPH

Implement:

• Friend requests

• Friend acceptance

• Friend removal

• Following

• Unfollowing

• Follow requests

• Suggested connections

• Mutual connections

• Blocked users

• Muted users

• Restricted users

• Relationship state lookup

• Privacy-aware graph queries

• Redis caching where approved

All relationship mutations must be idempotent where required.

Generate domain events for graph changes.

────────────────────────────────────────

POST SERVICE

Implement:

• Text posts

• Image posts

• Video posts

• Multi-media posts

• Link posts

• Rich link metadata boundaries

• Polls

• Check-ins

• Location posts

• Shared posts

• Reposts

• Quote sharing

• Collaborative posts

• Drafts

• Scheduled posts

• Publishing

• Editing

• Deletion

• Soft deletion

• Visibility

• Audience controls

• Privacy enforcement

• Mentions

• Hashtags

Every mutation must enforce:

• Authentication

• Authorization

• Audience visibility

• Validation

• Moderation state

────────────────────────────────────────

MEDIA SERVICE

Implement:

• Upload initialization

• Signed upload URL generation

• Upload validation

• Media ownership

• Metadata persistence

• Processing status

• Image processing integration

• Video processing integration

• Thumbnail generation

• Preview generation

• Metadata extraction

• Content lifecycle

• Deletion

• Quarantine support

• Malware scanning integration boundaries

• CDN delivery boundaries

Do not proxy large media uploads through ordinary application servers unless explicitly required.

────────────────────────────────────────

IMAGE PROCESSING

Generate workers supporting:

• Resize operations

• Responsive variants

• Format conversion

• Compression

• Thumbnail generation

• Metadata extraction

• Processing status updates

• Retry handling

• Dead-letter handling

• Idempotent processing

Use Sharp or approved architecture equivalents.

────────────────────────────────────────

VIDEO PROCESSING

Generate workers supporting:

• FFmpeg processing

• Transcoding

• Thumbnail generation

• Preview generation

• Duration extraction

• Metadata extraction

• Processing state tracking

• Retry handling

• Timeout handling

• Failed job recovery

Prepare architecture for adaptive bitrate streaming where approved.

────────────────────────────────────────

COMMENTS

Implement:

• Comment creation

• Replies

• Nested discussion structures

• Pagination

• Editing

• Deletion

• Soft deletion

• Mentions

• Moderation states

• Reporting integration

• Spam detection hooks

• Privacy enforcement

• Authorization

────────────────────────────────────────

REACTIONS

Implement:

• Multiple reaction types

• Add reaction

• Change reaction

• Remove reaction

• Idempotency

• Aggregate counters

• Event generation

• Cache invalidation

Design for extremely high write volumes.

────────────────────────────────────────

SHARING

Implement:

• Internal sharing

• Reposts

• Quote sharing

• Private sharing

• Group sharing

• External share metadata where applicable

• Visibility enforcement

• Engagement events

────────────────────────────────────────

FEED SERVICE

Implement the approved feed architecture.

Support:

• Personalized feeds

• Friends feeds

• Following feeds

• Group feeds

• Community feeds

• Page feeds

• Creator feeds

• Trending feeds

• Recommended feeds

• Sponsored-content integration boundaries

Implement:

• Candidate retrieval

• Fanout-on-write where approved

• Fanout-on-read where approved

• Hybrid strategies

• Ranking integration

• Privacy filtering

• Block filtering

• Deduplication

• Cursor pagination

• Cache strategy

• Feed invalidation

• Event-driven updates

Do not embed recommendation model logic directly into feed delivery.

────────────────────────────────────────

RECOMMENDATION SERVICE

Implement the modular recommendation boundaries.

Support:

• Candidate generation

• Feature retrieval interfaces

• Ranking integration

• Re-ranking

• Diversity

• Deduplication

• Privacy filtering

• Safety filtering

• Experimentation

• Feedback collection

• Recommendation event ingestion

Maintain provider and model independence.

────────────────────────────────────────

GROUP SERVICE

Implement:

• Public groups

• Private groups

• Hidden groups

• Membership

• Membership requests

• Invitations

• Roles

• Permissions

• Rules

• Announcements

• Pinned content

• Member management

• Moderation integration

• Group posts

• Group media

• Group event relationships

────────────────────────────────────────

COMMUNITY SERVICE

Implement the approved community model.

Support:

• Community creation

• Membership

• Roles

• Permissions

• Administration

• Moderation

• Community discovery

• Community content relationships

• Event-driven membership changes

────────────────────────────────────────

PAGE SERVICE

Implement:

• Public pages

• Creator pages

• Business pages

• Page ownership

• Team members

• Page roles

• Verification state

• Followers

• Content relationships

• Analytics event generation

────────────────────────────────────────

CREATOR SERVICE

Implement:

• Creator account capabilities

• Creator profile state

• Creator analytics boundaries

• Audience metrics boundaries

• Content metrics boundaries

• Monetization readiness

• Brand partnership readiness

• Creator permissions

────────────────────────────────────────

BUSINESS SERVICE

Implement:

• Business accounts

• Business profiles

• Ownership

• Team members

• Roles

• Verification workflows

• Business settings

• Content relationships

• Commerce boundaries

────────────────────────────────────────

EVENT SERVICE

Implement:

• Event creation

• Public events

• Private events

• Online events

• Physical events

• Hybrid events

• Invitations

• RSVPs

• Guest lists

• Event discussions

• Event media relationships

• Notifications integration

• Discovery integration

• Calendar integration boundaries

────────────────────────────────────────

MESSAGING SERVICE

Implement:

• One-to-one conversations

• Group conversations

• Page messaging

• Business messaging

• Conversation membership

• Message creation

• Text messages

• Media messages

• Voice message integration

• Reactions

• Replies

• Delivery state

• Read receipts

• Typing integration

• Message pagination

• Multi-device synchronization

• Offline synchronization

• Message deletion

• Moderation and reporting boundaries

Follow the approved encryption and privacy architecture.

────────────────────────────────────────

PRESENCE AND REAL-TIME

Implement:

• Socket.IO authentication

• Connection lifecycle

• Presence

• Online status

• Typing indicators

• Live notifications

• Message delivery events

• Heartbeats

• Connection recovery

• Distributed scaling

• Redis-backed coordination

• Connection limits

• Abuse protection

• Metrics

Implement graceful degradation when Redis or WebSocket coordination is temporarily unavailable.

────────────────────────────────────────

NOTIFICATION SERVICE

Implement:

• Notification creation

• Aggregation

• Deduplication

• Preferences

• Muting

• In-app notifications

• Push notification boundaries

• Email notification boundaries

• Desktop notification boundaries

• Delivery tracking

• Retry handling

• Failure handling

• Deep-link metadata

────────────────────────────────────────

SEARCH SERVICE

Implement event-driven indexing and search.

Support:

• Users

• Pages

• Creators

• Businesses

• Groups

• Communities

• Posts

• Videos

• Events

• Marketplace listings

• Hashtags

• Locations

Implement:

• Index creation

• Index versioning

• Aliases

• Reindexing

• Event-driven updates

• Deleted-content removal

• Privacy filtering

• Autocomplete

• Filters

• Ranking boundaries

• Search analytics

────────────────────────────────────────

MARKETPLACE SERVICE

Implement:

• Listings

• Listing categories

• Seller profiles

• Buyer interactions

• Listing media

• Location-aware discovery boundaries

• Search integration

• Filters

• Saved listings

• Availability

• Listing lifecycle

• Moderation

• Reporting

• Fraud detection hooks

• Buyer-seller messaging relationships

────────────────────────────────────────

COMMERCE SERVICE

Implement the approved commerce boundaries.

Support:

• Merchant profiles

• Product catalogs

• Product records

• Inventory boundaries

• Product media

• Promotions

• Coupons

• Checkout integration boundaries

• Orders

• Order lifecycle

• Refund integration boundaries

Do not tightly couple external payment provider logic into unrelated social domains.

────────────────────────────────────────

PAYMENT INTEGRATION SERVICE

Implement provider abstraction for approved payment providers.

Support:

• Payment intent creation

• Payment status synchronization

• Webhook verification

• Idempotency

• Refund boundaries

• Error handling

• Audit events

Never trust payment status supplied directly by clients.

────────────────────────────────────────

ADVERTISING SERVICE

Implement:

• Advertiser organizations

• Team members

• Ad accounts

• Campaigns

• Campaign objectives

• Ad sets

• Ads

• Creative assets

• Targeting configuration

• Audience relationships

• Budget configuration

• Scheduling

• Campaign lifecycle

• Review workflows

• Policy enforcement integration

• Experiment configuration

Maintain clear boundaries between:

• Campaign management

• Audience management

• Creative management

• Delivery

• Measurement

• Reporting

────────────────────────────────────────

AD DELIVERY

Implement the approved delivery architecture.

Support:

• Candidate selection

• Eligibility filtering

• Targeting evaluation

• Budget validation

• Frequency caps

• Pacing

• Ranking integration

• Experiment assignment

• Delivery events

• Impression tracking

• Click tracking

• Conversion ingestion boundaries

• Fraud detection integration

• Policy enforcement

Design high-volume operations with:

• Redis caching

• Idempotency

• Asynchronous event processing

• Failure isolation

Do not make core feed availability dependent on non-critical advertising analytics.

────────────────────────────────────────

ANALYTICS

Implement event ingestion and aggregation boundaries for:

• Product analytics

• Engagement analytics

• Content analytics

• Creator analytics

• Business analytics

• Marketplace analytics

• Advertising analytics

• Platform analytics

Support:

• Event validation

• Event versioning

• Privacy classification

• Deduplication

• Batch processing readiness

• Stream processing readiness

• Aggregation jobs

• Retention policies

Do not expose raw sensitive analytics data without authorization.

────────────────────────────────────────

MODERATION SERVICE

Implement:

• User reports

• Content reports

• Comment reports

• Message reports

• Group reports

• Page reports

• Marketplace reports

• Advertising reports

• Appeals

• Moderation queues

• Assignment

• Moderator notes

• Evidence references

• Moderation decisions

• Enforcement integration

• Audit logging

────────────────────────────────────────

TRUST AND SAFETY

Implement service boundaries and workflows for:

• Spam detection

• Abuse detection

• Fake account detection

• Bot detection

• Fraud detection

• Account takeover detection hooks

• Suspicious activity scoring

• Reputation scoring

• Risk scoring

• Human escalation

• Automated enforcement

• Event-driven detection

All automated decisions must support auditability and human-review workflows where approved.

────────────────────────────────────────

FEATURE FLAG SERVICE

Implement:

• Flag creation

• Flag evaluation

• Environment targeting

• User targeting

• Role targeting

• Geographic targeting

• Percentage rollout

• Kill switches

• Default values

• Audit history

• Change management

• Propagation

• Caching

• Safe fallback behavior

────────────────────────────────────────

AUDIT SERVICE

Implement immutable or append-oriented audit records for:

• Authentication events

• Authorization-sensitive actions

• Administrative actions

• Moderation actions

• Advertising changes

• Business changes

• Security-sensitive events

• Feature flag changes

Support:

• Actor identification

• Resource identification

• Action

• Timestamp

• Request correlation

• Before and after metadata where appropriate

• Privacy-aware data handling

────────────────────────────────────────

DEVELOPER PLATFORM

Implement foundations for:

• API clients

• API keys

• OAuth applications

• Scopes

• Webhooks

• Webhook subscriptions

• Signature verification

• Rate limiting

• Usage tracking

• Developer audit logging

• API versioning

────────────────────────────────────────

AI PLATFORM GATEWAY

Implement a provider-independent gateway architecture.

Support:

• Provider abstraction

• Request validation

• Authorization

• Rate limiting

• Model routing

• Prompt template references

• Usage tracking

• Cost tracking

• Caching where safe

• Safety checks

• Audit logging

• Evaluation hooks

Do not hardcode a specific AI provider into domain services.

────────────────────────────────────────

DATABASE IMPLEMENTATION

Implement the approved PostgreSQL and Prisma architecture.

Generate:

• Prisma schema organization

• Database migrations

• Foreign keys

• Constraints

• Unique indexes

• Composite indexes

• Partial indexes

• Partitioning preparation

• Database ownership documentation

• Read model support where required

• Connection management

• Transaction boundaries

Every service must clearly own its database entities.

Do not allow arbitrary cross-service direct database writes.

────────────────────────────────────────

REDIS IMPLEMENTATION

Implement Redis usage for approved use cases including:

• Caching

• Sessions

• Rate limiting

• Distributed locks

• Feed caching

• Relationship caching

• Presence

• Socket.IO coordination

• Feature flag caching

• Idempotency keys

Define:

• Key naming

• TTL policies

• Invalidation

• Serialization

• Failure behavior

• Metrics

────────────────────────────────────────

KAFKA OR REDPANDA IMPLEMENTATION

Implement:

• Topic configuration

• Producers

• Consumers

• Event contracts

• Schema versioning

• Partition keys

• Consumer groups

• Retry strategies

• Dead-letter topics

• Idempotent consumers

• Event tracing

• Error handling

• Privacy classification

Follow the approved event catalog.

────────────────────────────────────────

BULLMQ IMPLEMENTATION

Implement queues and workers for approved asynchronous workloads including:

• Image processing

• Video processing

• Notifications

• Search indexing

• Feed maintenance

• Recommendation processing

• Analytics aggregation

• Scheduled publishing

• Data retention

• Retry processing

• Dead-letter recovery

Implement:

• Retry policies

• Exponential backoff where appropriate

• Job idempotency

• Concurrency limits

• Timeouts

• Failure tracking

• Graceful shutdown

────────────────────────────────────────

API IMPLEMENTATION

Generate production-ready APIs.

Every endpoint must support, where applicable:

• Authentication

• Authorization

• Input validation

• Privacy enforcement

• Rate limiting

• Pagination

• Filtering

• Sorting

• Idempotency

• Structured errors

• Request correlation

Generate:

• Controllers

• DTOs

• Validation schemas

• Application services

• Domain services

• Repositories

• Guards

• Middleware

• Interceptors

• Exception filters

• OpenAPI documentation

Maintain backward compatibility.

────────────────────────────────────────

WEBSOCKET IMPLEMENTATION

Implement approved Socket.IO architecture.

Generate:

• Gateway modules

• Authentication

• Authorization

• Connection handling

• Room management

• Presence events

• Typing events

• Messaging events

• Notification events

• WebRTC signaling boundaries

• Heartbeats

• Reconnection support

• Distributed coordination

• Rate limiting

• Backpressure handling

• Metrics

────────────────────────────────────────

PRIVACY ENFORCEMENT

Implement server-side privacy enforcement across:

• Profiles

• Social graph

• Posts

• Comments

• Feed

• Search

• Recommendations

• Groups

• Messaging

• Marketplace

• Notifications

• Analytics

• Advertising

Never assume privacy rules are enforced only by clients.

────────────────────────────────────────

SECURITY REQUIREMENTS

Implement:

• JWT security

• Refresh token rotation

• Secure password hashing

• MFA

• Passkey readiness

• Session management

• RBAC

• Resource authorization

• Relationship-aware authorization

• Rate limiting

• Input validation

• SQL injection protection

• XSS-aware output boundaries

• CSRF protection where required

• Secure headers

• CORS

• SSRF protections

• Secure file upload validation

• Malware scanning integration

• Secrets isolation

• Audit logging

• Abuse protection

Follow OWASP best practices.

────────────────────────────────────────

TESTING

Generate tests continuously with implementation.

Include:

• Unit tests

• Repository tests

• Service tests

• Controller tests

• Integration tests

• API tests

• Authentication tests

• Authorization tests

• Privacy tests

• Event contract tests

• Kafka integration tests

• Redis integration tests

• Queue tests

• WebSocket tests

• Database tests

• Performance test architecture

• Load test readiness

Do not defer all tests until the end.

────────────────────────────────────────

IMPLEMENTATION ORDER

Implement incrementally in this approximate order while respecting architecture dependencies:

Milestone Group 1

• Monorepo foundation

• Shared packages

• Configuration

• Logging

• Error handling

• Validation

• Database foundation

• Redis foundation

• Kafka foundation

• Queue foundation

• Observability foundation

Milestone Group 2

• Authentication

• Authorization

• Identity

• Sessions

• Devices

• Users

• Profiles

Milestone Group 3

• Social graph

• Friendships

• Following

• Blocking

• Privacy foundations

Milestone Group 4

• Media

• Image processing

• Video processing

• Posts

• Comments

• Reactions

• Sharing

Milestone Group 5

• Feed

• Recommendations

• Ranking integration boundaries

Milestone Group 6

• Groups

• Communities

• Pages

• Creators

• Businesses

• Events

Milestone Group 7

• Messaging

• Presence

• WebSockets

• Real-time notifications

Milestone Group 8

• Search

• Discovery

Milestone Group 9

• Marketplace

• Commerce

• Payment integration boundaries

Milestone Group 10

• Advertising

• Ad delivery

• Measurement

• Reporting

Milestone Group 11

• Moderation

• Trust & Safety

• Spam detection

• Fraud detection

• Appeals

Milestone Group 12

• Analytics

• Feature flags

• Audit

• Developer platform

• AI platform gateway

Milestone Group 13

• Backend hardening

• Performance testing

• Security testing

• Integration validation

• Documentation

────────────────────────────────────────

PROJECT INDEX

Maintain a living Backend Project Index.

After every milestone update:

• Current milestone

• Completed services

• Completed modules

• Completed APIs

• Completed database objects

• Completed Prisma models

• Completed migrations

• Completed Redis components

• Completed Kafka topics

• Completed event producers

• Completed event consumers

• Completed queues

• Completed WebSocket domains

• Completed tests

• Remaining work

• Dependencies

• Known risks

• Exact next file

────────────────────────────────────────

OUTPUT FORMAT

For every generated file provide:

1. Exact file path
2. Complete file contents

Never generate pseudo-code.

Never generate placeholders.

Never generate TODO comments.

Never omit implementations.

Never say:

• "implement similarly"

• "left as an exercise"

• "for brevity"

• "remaining code omitted"

Every generated file must compile and integrate with previously generated files.

Do not regenerate unchanged files.

Only modify files when required.

────────────────────────────────────────

STOP CONDITIONS

Implement the backend incrementally.

Each milestone should contain approximately 20–40 files.

At the end of every milestone:

1. Verify compilation consistency.
2. Verify dependency consistency.
3. Verify API contract consistency.
4. Verify database ownership.
5. Verify event contract consistency.
6. Verify security requirements for the completed milestone.
7. Update the Backend Project Index.
8. List completed services and features.
9. Identify the exact next file or logical implementation unit.

STOP.

Wait for approval before generating the next milestone.

The next prompt after backend implementation will be:

Project 4 — Enterprise Facebook-Style Social Platform
Frontend Prompt
