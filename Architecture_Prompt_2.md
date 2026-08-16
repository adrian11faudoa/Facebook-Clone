Using the approved Architecture Prompt — Volume 1 and the Master Prompt above.

Continue from the exact stopping point.

DO NOT begin backend implementation.

DO NOT generate application source code.

This is Architecture Prompt — Volume 2.

Complete the remaining enterprise architecture required before Backend, Frontend, Mobile, and Infrastructure implementation begins.

The architecture generated in Volume 1 and Volume 2 together becomes the authoritative blueprint for the entire project.

Do not redesign decisions already approved in Volume 1 unless a critical inconsistency, scalability issue, security issue, or operational risk requires a correction.

If a previous decision must be changed, explicitly document:

1. Previous decision.
2. Problem identified.
3. Proposed replacement.
4. Impact on dependent services.
5. Migration or compatibility strategy.

────────────────────────────────────────

ADVERTISING PLATFORM

Design a complete advertising architecture supporting:

• Advertiser Accounts

• Advertising Organizations

• Team Members

• Roles and Permissions

• Ad Accounts

• Campaigns

• Campaign Objectives

• Ad Sets

• Ads

• Creative Assets

• Images

• Videos

• Text Variations

• Call-to-Action Configuration

• Landing Destinations

• Audience Targeting

• Geographic Targeting

• Demographic Targeting

• Interest Targeting

• Behavioral Targeting

• Custom Audiences

• Lookalike Audience Architecture

• Exclusion Audiences

• Budgeting

• Daily Budgets

• Lifetime Budgets

• Bid Strategies

• Scheduling

• Campaign States

• Review and Approval

• Ad Moderation

• Delivery

• Frequency Controls

• Pacing

• Experimentation

• A/B Testing

• Reporting

• Billing Integration Boundaries

• Conversion Tracking

• Attribution Architecture

Design clear domain boundaries between:

Advertising Management

Ad Delivery

Audience Management

Creative Management

Billing

Measurement

Attribution

Reporting

Do not tightly couple advertising delivery to the core social feed service.

────────────────────────────────────────

AD DELIVERY ARCHITECTURE

Design an independent ad delivery system supporting:

• Candidate Selection

• Eligibility Filtering

• Targeting Evaluation

• Budget Validation

• Frequency Capping

• Pacing

• Ranking

• Auction Readiness

• Experiment Assignment

• Delivery Logging

• Impression Tracking

• Click Tracking

• Conversion Event Ingestion

• Fraud Detection Integration

• Policy Enforcement

Support extremely high request volumes.

Clearly define:

• Synchronous request path.

• Asynchronous processing path.

• Cache strategy.

• Event generation.

• Analytics pipeline.

• Failure behavior.

• Privacy enforcement.

• Idempotency requirements.

────────────────────────────────────────

RECOMMENDATION PLATFORM

Design a modular recommendation architecture supporting:

• Feed Recommendations

• People Recommendations

• Friend Suggestions

• Group Recommendations

• Community Recommendations

• Page Recommendations

• Creator Recommendations

• Event Recommendations

• Marketplace Recommendations

• Content Recommendations

• Video Recommendations

• Local Recommendations

• Advertising Recommendations where permitted

Design independent layers for:

• Candidate Generation

• Feature Retrieval

• Feature Engineering

• Ranking

• Re-ranking

• Diversity

• Deduplication

• Safety Filtering

• Privacy Filtering

• Experimentation

• Feedback Collection

• Model Serving Readiness

The recommendation platform must allow future ML models to evolve without requiring major rewrites of core social services.

────────────────────────────────────────

AI PLATFORM ARCHITECTURE

Design a provider-independent AI platform.

Support future capabilities including:

• Content Recommendations

• Natural Language Search

• Content Summarization

• Caption Assistance

• Translation

• Accessibility Descriptions

• Image Understanding

• Video Understanding

• Spam Detection

• Fraud Detection

• Moderation Assistance

• Trust & Safety Assistance

• Creator Assistance

• Business Assistance

• Community Assistance

• Customer Support Assistance

• Developer Assistance

Design:

• AI Gateway

• Model Provider Abstraction

• Prompt Management

• Model Routing

• Request Validation

• Rate Limiting

• Usage Tracking

• Cost Tracking

• Caching

• Evaluation

• Safety Controls

• Human Review Integration

• Audit Logging

• Data Privacy Controls

• Model Versioning

• Experimentation

Do not hardcode a specific AI provider into the platform architecture.

Sensitive user data must not be exposed to AI providers without explicit policy and authorization controls.

────────────────────────────────────────

FEATURE FLAG ARCHITECTURE

Design a centralized feature flag system supporting:

• Environment-specific Flags

• User Targeting

• Role Targeting

• Geographic Targeting

• Percentage Rollouts

• A/B Experiments

• Kill Switches

• Dependency Management

• Default Values

• Offline Behavior

• Client-side Evaluation where safe

• Server-side Evaluation

• Audit History

• Change Approval

• Rollback

• Analytics Integration

Define how feature flags propagate to:

• Backend Services

• Web Applications

• Mobile Applications

• Background Workers

────────────────────────────────────────

MODERATION ARCHITECTURE

Design a complete moderation system.

Support:

• User Reports

• Content Reports

• Comment Reports

• Message Reports

• Group Reports

• Page Reports

• Marketplace Reports

• Advertising Reports

• Spam Reports

• Fraud Reports

• Appeals

• Moderator Assignments

• Moderation Queues

• Automated Detection

• Human Review

• Enforcement Actions

• Temporary Restrictions

• Permanent Restrictions

• Content Removal

• Content Visibility Reduction

• Account Suspension

• Account Termination

• Warning Systems

• Strike Systems

• Appeal Review

• Moderator Notes

• Evidence Storage

• Audit Trails

Clearly separate:

Moderation Decisions

Policy Definitions

Automated Detection

Human Review

Enforcement

Appeals

Audit

────────────────────────────────────────

TRUST AND SAFETY

Design systems supporting:

• Abuse Detection

• Coordinated Abuse Detection

• Spam Detection

• Fake Account Detection

• Bot Detection

• Fraud Detection

• Account Takeover Detection

• Suspicious Login Detection

• Impersonation Detection

• Harassment Detection

• Harmful Content Detection

• Marketplace Fraud Detection

• Advertising Fraud Detection

• Rate Abuse Detection

• Reputation Systems

• Risk Scoring

• Human Escalation

• Automated Enforcement

• Security Incident Integration

Design event flows between Trust & Safety systems and:

Authentication

Social Graph

Posts

Comments

Messaging

Marketplace

Advertising

Moderation

Audit

────────────────────────────────────────

PRIVACY ARCHITECTURE

Design a privacy-first architecture.

Support:

• Profile Privacy

• Audience Selection

• Post Visibility

• Friend Visibility

• Follower Visibility

• Location Privacy

• Search Visibility

• Contact Discovery Controls

• Messaging Permissions

• Blocking

• Restricting

• Muting

• Data Export

• Account Deletion

• Data Retention Policies

• Consent Management

• Analytics Consent

• Advertising Preferences

• Personalization Controls

• AI Data Controls

Define how privacy rules are enforced consistently across:

• API Gateway

• Backend Services

• Feed Generation

• Search

• Recommendations

• Notifications

• Messaging

• Analytics

• Advertising

• AI Systems

Privacy filtering must not rely exclusively on frontend enforcement.

────────────────────────────────────────

AUTHENTICATION ARCHITECTURE

Complete the authentication architecture.

Support:

• Registration

• Login

• Logout

• Email Verification

• Phone Verification

• Password Authentication

• Password Reset

• OAuth

• Social Login

• Refresh Tokens

• Access Tokens

• Session Management

• Multi-device Sessions

• Device Management

• Session Revocation

• Suspicious Login Detection

• Multi-factor Authentication

• Authenticator Apps

• Recovery Codes

• Passkeys

• Account Recovery

• Rate Limiting

• Credential Stuffing Protection

• Brute-force Protection

• Security Notifications

Define:

• Token lifecycle.

• Session lifecycle.

• Refresh rotation.

• Device trust.

• Token revocation.

• Key rotation.

• Failure handling.

• Cross-service authentication.

────────────────────────────────────────

AUTHORIZATION ARCHITECTURE

Design authorization using:

• RBAC

• Resource-level permissions

• Relationship-aware permissions

• Organization permissions

• Group permissions

• Page permissions

• Business permissions

• Marketplace permissions

• Advertising permissions

• Administrative permissions

• Moderator permissions

• Service-to-service permissions

Support future policy-based authorization where required.

Define centralized and distributed authorization boundaries.

────────────────────────────────────────

EVENT-DRIVEN ARCHITECTURE

Use Kafka or Redpanda as the primary event backbone.

Generate a complete event catalog.

Include events for:

Identity

• UserRegistered

• UserVerified

• UserLoggedIn

• UserLoggedOut

• PasswordChanged

• SessionRevoked

Profiles

• ProfileCreated

• ProfileUpdated

• ProfileDeleted

Social Graph

• FriendRequested

• FriendAccepted

• FriendRemoved

• UserFollowed

• UserUnfollowed

• UserBlocked

Posts

• PostCreated

• PostUpdated

• PostDeleted

• PostPublished

• PostShared

Media

• MediaUploaded

• MediaProcessed

• MediaFailed

• MediaDeleted

Engagement

• CommentCreated

• CommentUpdated

• CommentDeleted

• ReactionCreated

• ReactionRemoved

Groups

• GroupCreated

• GroupUpdated

• GroupMemberJoined

• GroupMemberRemoved

Pages

• PageCreated

• PageUpdated

• PageFollowed

Events

• EventCreated

• EventUpdated

• EventRSVPChanged

Messaging

• ConversationCreated

• MessageSent

• MessageDelivered

• MessageRead

• MessageDeleted

Notifications

• NotificationRequested

• NotificationSent

• NotificationDelivered

• NotificationFailed

Marketplace

• ListingCreated

• ListingUpdated

• ListingPublished

• ListingSold

Advertising

• CampaignCreated

• CampaignActivated

• AdImpressionRecorded

• AdClicked

• ConversionRecorded

Moderation

• ContentReported

• ModerationDecisionCreated

• EnforcementApplied

• AppealSubmitted

Analytics

• AnalyticsEventRecorded

• AggregationCompleted

Feature Flags

• FeatureFlagUpdated

AI

• AIRequestCreated

• AIRequestCompleted

• AIRequestFailed

For every event category define:

• Producer

• Consumer

• Event Schema

• Event Version

• Partition Key

• Ordering Requirements

• Retention

• Retry Strategy

• Dead-letter Handling

• Idempotency Strategy

• Privacy Classification

• Schema Evolution Rules

────────────────────────────────────────

CQRS ARCHITECTURE

Identify domains where CQRS is appropriate.

Evaluate:

• Feed

• Search

• Recommendations

• Analytics

• Notifications

• Advertising

• Moderation

• Marketplace Discovery

Clearly distinguish:

• Command Models

• Query Models

• Read Models

• Eventual Consistency Boundaries

• Projection Rebuilding

• Replay Requirements

Do not introduce CQRS into simple domains without a clear technical benefit.

────────────────────────────────────────

API ARCHITECTURE

Design complete API boundaries.

Support:

• REST APIs

• WebSocket APIs

• Internal Service APIs

• Event-based APIs

• Public Developer APIs

Define:

• API Versioning

• Authentication

• Authorization

• Pagination

• Cursor Pagination

• Filtering

• Sorting

• Error Models

• Validation

• Idempotency

• Rate Limiting

• Request Correlation

• Deprecation Strategy

• Backward Compatibility

• OpenAPI Documentation

Generate a high-level API contract catalog for every major domain.

Do not implement controllers or application code yet.

────────────────────────────────────────

WEBSOCKET ARCHITECTURE

Design the real-time architecture supporting:

• Authentication

• Authorization

• Connection Lifecycle

• Presence

• Typing

• Messaging

• Notifications

• Live Updates

• WebRTC Signaling

• Connection Recovery

• Heartbeats

• Distributed Socket Scaling

• Redis-backed Coordination

• Backpressure

• Connection Limits

• Abuse Protection

• Metrics

• Graceful Reconnection

Define:

• Namespaces.

• Rooms.

• Event contracts.

• Authentication lifecycle.

• Scaling model.

• Failure behavior.

────────────────────────────────────────

SEARCH ARCHITECTURE

Complete the search architecture.

Define indexes for:

• Users

• Pages

• Creators

• Businesses

• Groups

• Communities

• Posts

• Videos

• Events

• Marketplace Listings

• Hashtags

• Locations

Define:

• Indexing pipelines.

• Event-driven indexing.

• Reindexing.

• Index versioning.

• Alias switching.

• Ranking.

• Personalization.

• Privacy filtering.

• Deleted content handling.

• Synonym support.

• Autocomplete.

• Typo tolerance.

• Capacity scaling.

────────────────────────────────────────

ANALYTICS ARCHITECTURE

Design an analytics platform supporting:

Product Analytics

• Daily Active Users

• Monthly Active Users

• Retention

• Engagement

• Session Metrics

Content Analytics

• Post Views

• Video Views

• Shares

• Reactions

• Comments

Creator Analytics

• Audience Growth

• Reach

• Engagement

Business Analytics

• Page Performance

• Content Performance

Marketplace Analytics

• Listing Views

• Messages

• Sales Events

Advertising Analytics

• Impressions

• Reach

• Frequency

• Clicks

• Conversions

Platform Analytics

• API Latency

• Error Rates

• Queue Metrics

• Database Metrics

• Cache Metrics

• WebSocket Metrics

Define:

• Event collection.

• Event schemas.

• Data pipelines.

• Stream processing readiness.

• Aggregation.

• Data retention.

• Privacy controls.

• Reporting boundaries.

────────────────────────────────────────

DATA LIFECYCLE

Define data lifecycle policies for:

• User Accounts

• Posts

• Comments

• Messages

• Media

• Notifications

• Analytics Events

• Audit Logs

• Moderation Evidence

• Marketplace Data

• Advertising Data

Support:

• Active Data

• Archived Data

• Expired Data

• Deleted Data

• Legal Hold readiness

• Data Export

• Account Deletion

• Retention Policies

• Storage Lifecycle Policies

────────────────────────────────────────

MULTI-REGION ARCHITECTURE

Design a global deployment strategy.

Define:

• Primary Region

• Secondary Regions

• Regional Kubernetes Clusters

• Global Traffic Routing

• Health-based Failover

• CDN Edge Delivery

• Regional API Endpoints

• Regional Service Deployment

• Database Replication

• Read Replica Placement

• Cross-region Backup

• Object Replication

• Kafka Replication

• Search Replication

• Cache Isolation

Clearly classify workloads as:

• Active-Active

• Active-Passive

• Single Writer

• Multi-writer with Conflict Resolution

Do not assume all relational data can safely use multi-region multi-writer architecture.

────────────────────────────────────────

DISASTER RECOVERY

Define:

• Recovery Point Objectives

• Recovery Time Objectives

• Service Failure Recovery

• Availability Zone Failure

• Regional Failure

• Database Failure

• Redis Failure

• Kafka Failure

• Search Failure

• Object Storage Failure

• Kubernetes Cluster Failure

• CDN Failure

• DNS Failure

• Secrets Management Failure

• Security Incident Recovery

Generate a disaster recovery strategy including:

• Backups

• Restore Procedures

• Failover

• Failback

• Data Integrity Verification

• Recovery Testing

• Disaster Recovery Runbooks

────────────────────────────────────────

SECURITY ARCHITECTURE

Complete the enterprise security architecture.

Include:

• Zero Trust Principles

• Defense in Depth

• Identity Security

• Service Authentication

• Mutual TLS readiness

• Network Segmentation

• Encryption in Transit

• Encryption at Rest

• Key Management

• Secret Management

• API Security

• Rate Limiting

• Abuse Prevention

• DDoS Protection

• Web Application Firewall readiness

• Input Validation

• Output Encoding

• CSRF Protection

• XSS Protection

• SQL Injection Protection

• SSRF Protection

• Secure File Uploads

• Malware Scanning

• Dependency Security

• Container Security

• Infrastructure Security

• Audit Logging

• Security Monitoring

• Incident Response

Align architecture with OWASP best practices.

────────────────────────────────────────

OBSERVABILITY ARCHITECTURE

Design observability across the complete platform.

Metrics

• Application Metrics

• Infrastructure Metrics

• Database Metrics

• Redis Metrics

• Kafka Metrics

• Search Metrics

• Queue Metrics

• WebSocket Metrics

• Media Processing Metrics

• Business Metrics

Logging

• Structured Logging

• Centralized Collection

• Correlation IDs

• Privacy-aware Logging

Tracing

• OpenTelemetry

• Distributed Tracing

• HTTP Trace Propagation

• Kafka Trace Propagation

• Queue Trace Propagation

• WebSocket Trace Correlation

Define:

• SLIs

• SLOs

• Error Budgets

• Alerting

• Dashboard Architecture

• Incident Correlation

────────────────────────────────────────

INFRASTRUCTURE OVERVIEW

Design the high-level infrastructure architecture for:

• Local Development

• Development

• Staging

• Production

Include:

• Docker

• Docker Compose

• Kubernetes

• Helm

• Terraform

• GitHub Actions

• Container Registry

• Artifact Promotion

• Environment Configuration

• Secret Injection

• Database Migrations

• Progressive Delivery

• Canary Deployment readiness

• Blue-Green Deployment readiness

• Rollback Strategy

Do not generate the infrastructure files yet.

That will be implemented in the Infrastructure Prompt.

────────────────────────────────────────

MONOREPO STRUCTURE

Generate the complete final monorepo structure.

Include:

apps/

services/

packages/

infrastructure/

docs/

scripts/

testing/

For each major directory define:

• Purpose.

• Ownership boundaries.

• Dependency rules.

• Import rules.

• Shared package strategy.

Prevent inappropriate coupling between services.

────────────────────────────────────────

IMPLEMENTATION ROADMAP

Create the implementation sequence after architecture approval.

Organize:

Phase 1

Foundation

Phase 2

Identity and User Platform

Phase 3

Social Graph

Phase 4

Posts and Media

Phase 5

Engagement

Phase 6

Feed and Recommendations

Phase 7

Groups, Communities, Pages, and Events

Phase 8

Messaging and Real-Time Systems

Phase 9

Marketplace and Commerce

Phase 10

Advertising Platform

Phase 11

Search and Discovery

Phase 12

Notifications

Phase 13

Moderation and Trust & Safety

Phase 14

Analytics

Phase 15

AI Platform Readiness

Phase 16

Frontend and Mobile Applications

Phase 17

Infrastructure and DevOps

Phase 18

Testing, Performance, Security, and Production Hardening

For every phase define:

• Services involved.

• Major dependencies.

• Database dependencies.

• Event dependencies.

• API dependencies.

• Risk areas.

• Scalability considerations.

────────────────────────────────────────

PROJECT INDEX

Generate and maintain the final Architecture Project Index.

Include:

Approved Architecture Decisions

Applications

Domains

Bounded Contexts

Microservices

Database Components

Core Tables

Redis Components

Kafka Topics

Event Producers

Event Consumers

Search Indexes

Queues

External Integrations

API Domains

WebSocket Domains

Security Components

Observability Components

Infrastructure Components

Implementation Phases

Dependencies

Risks

Future Extensions

────────────────────────────────────────

ARCHITECTURE VALIDATION

Before completing this phase, perform an internal architecture consistency review.

Validate:

• No major feature lacks an owning domain.

• No critical service has undefined boundaries.

• Service responsibilities do not unnecessarily overlap.

• Database ownership is clear.

• Event producers and consumers are defined.

• High-volume paths have scaling strategies.

• Privacy enforcement is not dependent on frontend behavior.

• Security boundaries are defined.

• Failure behavior is considered.

• Multi-region assumptions are realistic.

• Disaster recovery covers critical dependencies.

• Backend implementation can proceed without redesigning the architecture.

────────────────────────────────────────

FINAL OUTPUT

Generate the complete architecture specification for Volume 2.

Include:

1. Remaining domain architecture.
2. Advertising architecture.
3. Recommendation architecture.
4. AI platform architecture.
5. Feature flag architecture.
6. Moderation architecture.
7. Trust and Safety architecture.
8. Privacy architecture.
9. Authentication architecture.
10. Authorization architecture.
11. Complete event architecture.
12. CQRS decisions.
13. API architecture.
14. WebSocket architecture.
15. Search architecture.
16. Analytics architecture.
17. Data lifecycle.
18. Multi-region architecture.
19. Disaster recovery.
20. Security architecture.
21. Observability architecture.
22. Infrastructure overview.
23. Final monorepo structure.
24. Implementation roadmap.
25. Final Architecture Project Index.

Do NOT implement backend code.

STOP after completing the architecture.

Wait for approval.

The next prompt after approval will be:

Project 4 — Enterprise Facebook-Style Social Platform
Backend Prom

Using the approved Architecture Blueprint — Volume 1 and the Master Prompt above.

Continue Phase 1 architecture.

Do NOT generate implementation code.

Continue from the exact stopping point.

This volume completes the enterprise architecture and becomes the definitive blueprint for Backend, Frontend, Mobile, AI, Infrastructure, Security, DevOps, and Operations.

────────────────────────────────────────

SEARCH PLATFORM

Generate complete architecture for:

• User Search

• Creator Search

• Business Search

• Post Search

• Reels Search

• Stories Search

• Hashtag Search

• Audio Search

• Location Search

• Comment Search

• Semantic Search (future-ready)

• AI Search (future-ready)

Support:

Autocomplete

Trending Searches

Search Suggestions

Typo Tolerance

Geo-aware Ranking

Language-aware Search

Personalized Ranking

Search Analytics

────────────────────────────────────────

MESSAGING

Design architecture supporting:

• One-to-One Chats

• Group Chats

• Creator Channels

• Vanishing Messages

• Voice Messages

• Images

• Videos

• Documents

• GIFs

• Stickers

• Emoji Reactions

• Read Receipts

• Typing Indicators

• Online Presence

• Scheduled Messages

• Message Search

────────────────────────────────────────

NOTIFICATIONS

Generate architecture for:

Push Notifications

In-app Notifications

Email Notifications

SMS Notifications (future-ready)

Creator Alerts

Business Alerts

Follower Alerts

Comment Alerts

Like Alerts

Mention Alerts

Message Alerts

Live Stream Alerts

Marketing Notifications

Notification Preferences

────────────────────────────────────────

LIVE STREAMING

Generate architecture supporting:

Live Broadcast

Multi-host Streaming

Live Chat

Pinned Comments

Moderation Queue

Viewer Analytics

Replay Storage

Recording Pipeline

Adaptive Bitrate Streaming

Low-Latency Delivery

Future Live Commerce

────────────────────────────────────────

CREATOR PLATFORM

Design complete architecture for:

Creator Profiles

Creator Verification

Creator Dashboard

Creator Analytics

Audience Insights

Revenue Analytics

Content Scheduling

Brand Partnerships

Campaign Management

Creator Marketplace

Affiliate Platform

Digital Products

Memberships (future-ready)

────────────────────────────────────────

BUSINESS PLATFORM

Support:

Business Profiles

Business Verification

Business Insights

Advertising

Promotions

Product Catalog

Commerce Integration

Lead Generation

CRM Integrations

Marketing Analytics

────────────────────────────────────────

COMMERCE

Generate architecture supporting:

Product Catalog

Product Tagging

Shopping Posts

Checkout Integration

Order Tracking

Inventory Sync

Coupons

Discount Campaigns

Merchant APIs

Future Marketplace Expansion

────────────────────────────────────────

ADVERTISING PLATFORM

Generate architecture for:

Campaign Management

Audience Segmentation

Budget Management

Auction-ready Design

Ad Delivery

Ad Targeting

Sponsored Posts

Sponsored Stories

Sponsored Reels

Performance Analytics

Billing Integration

Fraud Detection

────────────────────────────────────────

MODERATION

Design architecture supporting:

User Reporting

Content Reporting

Spam Detection

Bot Detection

Fake Account Detection

NSFW Detection

Copyright Detection

Community Moderation

Appeals

Moderator Dashboard

Trust & Safety

────────────────────────────────────────

SECURITY

Generate architecture for:

JWT Authentication

OAuth

Refresh Tokens

Passkeys (future-ready)

Multi-factor Authentication

RBAC

ABAC (future-ready)

Rate Limiting

Fraud Detection

Account Recovery

Device Management

Session Validation

Encryption at Rest

Encryption in Transit

OWASP Compliance

────────────────────────────────────────

ANALYTICS

Generate architecture supporting:

Daily Active Users

Monthly Active Users

Engagement Metrics

Feed Performance

Creator Analytics

Business Analytics

Revenue Metrics

Advertising Metrics

Video Completion Rate

Story Completion Rate

Livestream Metrics

Recommendation Metrics

Platform Health

────────────────────────────────────────

AI PLATFORM

Prepare architecture for:

Recommendation Models

Ranking Models

Vision Models

Content Moderation AI

Semantic Search

Caption Generation

Automatic Hashtags

Creator Assistant

Advertising Optimization

Content Quality Scoring

AI Feature Store

Prompt Management

LLM Gateway

Model Registry

Inference Services

AI Audit Logs

────────────────────────────────────────

EVENT-DRIVEN ARCHITECTURE

Use Kafka (or Redpanda) as the event backbone.

Generate events for:

UserRegistered

ProfileUpdated

FollowCreated

FollowRemoved

PostCreated

PostEdited

PostDeleted

StoryPublished

StoryExpired

ReelUploaded

VideoProcessed

MediaUploaded

MediaProcessed

CommentCreated

CommentDeleted

ReactionAdded

ReactionRemoved

CollectionCreated

MessageSent

NotificationQueued

CreatorVerified

BusinessVerified

CampaignCreated

AdvertisementDelivered

RecommendationGenerated

ReportSubmitted

ModerationCompleted

AnalyticsUpdated

Generate producers, consumers, retry strategies, dead-letter topics, idempotency rules, and event versioning.

────────────────────────────────────────

DEPLOYMENT ARCHITECTURE

Generate:

Multi-region Kubernetes Topology

Regional API Gateways

Global CDN Architecture

Media Processing Clusters

Background Worker Clusters

Recommendation Clusters

Search Clusters

Analytics Clusters

Disaster Recovery

Zero-downtime Deployment Strategy

Autoscaling Strategy

────────────────────────────────────────

INFRASTRUCTURE OVERVIEW

Design infrastructure for:

Docker

Kubernetes

Helm

Terraform

GitHub Actions

Redis

Kafka

Elasticsearch

PostgreSQL

S3-compatible Storage

CloudFront

Vault

Prometheus

Grafana

Loki

Tempo

OpenTelemetry

────────────────────────────────────────

PHASE 1 REQUIREMENTS

Generate ONLY:

1. Complete Enterprise System Architecture
2. Domain Decomposition
3. Bounded Contexts
4. Service Boundaries
5. Monorepo Structure
6. Folder Hierarchy
7. ERD
8. PostgreSQL Schema
9. Prisma Schema
10. Redis Architecture
11. Kafka Event Catalog
12. Elasticsearch Mappings
13. Queue Architecture
14. API Contracts
15. WebSocket Architecture
16. Authentication Architecture
17. Authorization Model
18. Recommendation Architecture
19. Feed Generation Architecture
20. Media Processing Pipeline
21. Search Architecture
22. Live Streaming Architecture
23. Deployment Architecture
24. Kubernetes Topology
25. Infrastructure Overview
26. Security Architecture
27. AI Platform Architecture
28. Disaster Recovery Strategy
29. Project Index

Do NOT implement backend code.

STOP after Phase 1.

Wait for approval before backend implementation.

────────────────────────────────────────

ARCHITECTURAL DECISIONS

Unless there is a compelling technical reason otherwise, assume:

• NestJS for backend services

• PostgreSQL + Prisma for transactional data

• Redis for caching, sessions, distributed locks, and feed caching

• Kafka (or Redpanda) for event streaming

• BullMQ for asynchronous processing

• Socket.IO for real-time messaging

• Elasticsearch/OpenSearch for search

• AWS S3-compatible storage for media

• CloudFront for CDN

• FFmpeg for video processing

• Sharp for image processing

• Kubernetes for orchestration

• Terraform for Infrastructure as Code

• OpenTelemetry for observability

• Vault for secrets management

• Event-driven communication where appropriate

• CQRS where appropriate

• Clean Architecture

• Domain-Driven Design

• Repository Pattern

• Dependency Injection

Design every architectural decision for long-term scalability, maintainability, resilience, creator monetization, business growth, AI integration, and global deployment.
