Using the Master Prompt above.

DO NOT begin implementation.

Your responsibility in this phase is to design the complete enterprise architecture for a production-ready global social networking platform supporting individuals, communities, creators, businesses, messaging, content distribution, events, commerce, advertising, and future AI-powered experiences.

The goal is NOT to clone any existing platform.

Build an independent, scalable, cloud-native social ecosystem with enterprise-grade architecture.

This architecture becomes the single source of truth for Backend, Frontend, Mobile, Infrastructure, DevOps, Security, Data Engineering, AI, QA, and Operations.

Do NOT generate source code.

Generate only architecture, engineering specifications, domain models, service boundaries, infrastructure decisions, API contracts, event architecture, deployment topology, scalability strategies, security models, data architecture, recommendation architecture, and implementation plans.

────────────────────────────────────────

MISSION

Build a production-ready global social networking platform supporting:

• User Profiles

• Social Graphs

• Friends

• Followers

• Posts

• Media

• Comments

• Reactions

• Shares

• Groups

• Communities

• Pages

• Creators

• Businesses

• Events

• Messaging

• Voice and Video Communication

• News Feed

• Recommendations

• Search

• Marketplace

• Commerce

• Advertising

• Notifications

• Moderation

• Trust & Safety

• Analytics

• Developer Platform

• AI-powered features

Design for:

• 1B+ registered users

• Hundreds of millions of daily active users

• Billions of social interactions

• Billions of posts and comments

• Billions of media objects

• Millions of concurrent real-time connections

• Global multi-region deployment

• Active-active architecture where appropriate

• High availability

• Horizontal scaling

• Zero-downtime deployments

• Long-term maintainability

────────────────────────────────────────

PRIMARY TECHNOLOGY STACK

Frontend

• Next.js 15

• React 19

• TypeScript

• Tailwind CSS

Mobile

• React Native

• Expo

• TypeScript

Backend

• Node.js

• NestJS

• TypeScript

Database

• PostgreSQL

• Prisma ORM

Caching

• Redis

Realtime

• Socket.IO

• WebSockets

Event Streaming

• Kafka or Redpanda

Background Jobs

• BullMQ

Search

• Elasticsearch or OpenSearch

Object Storage

• AWS S3-compatible storage

CDN

• CloudFront-compatible CDN

Media Processing

• FFmpeg

• Sharp

Voice and Video

• WebRTC

Infrastructure

• Docker

• Kubernetes

• Helm

• Terraform

• GitHub Actions

Observability

• Prometheus

• Grafana

• Loki

• Tempo

• OpenTelemetry

Secrets Management

• HashiCorp Vault

────────────────────────────────────────

APPLICATIONS

Design complete architecture for:

• Consumer Mobile Application

• Consumer Web Application

• Creator Dashboard

• Business Dashboard

• Community Administration Dashboard

• Marketplace Seller Dashboard

• Advertising Manager

• Administration Dashboard

• Moderation Dashboard

• Internal Operations Dashboard

• Public API

• Developer Portal

────────────────────────────────────────

USER TYPES

Support:

Guest

Registered User

Verified User

Creator

Professional Creator

Page Administrator

Business Owner

Business Team Member

Group Administrator

Group Moderator

Marketplace Seller

Marketplace Buyer

Advertiser

Developer

Moderator

Trust & Safety Operator

Platform Administrator

System Service

────────────────────────────────────────

CORE DOMAINS

Generate architecture and bounded contexts for:

Identity

Authentication

Authorization

Users

Profiles

Social Graph

Friendships

Followers

Posts

Media

Comments

Reactions

Sharing

News Feed

Recommendations

Groups

Communities

Pages

Creators

Businesses

Events

Messaging

Presence

Notifications

Search

Marketplace

Commerce

Advertising

Payments

Analytics

Moderation

Trust & Safety

Spam Detection

Fraud Detection

Feature Flags

Audit

Developer Platform

AI Platform

────────────────────────────────────────

MICROSERVICES

Generate service boundaries for:

API Gateway

Authentication Service

Authorization Service

Identity Service

User Service

Profile Service

Social Graph Service

Friendship Service

Follow Service

Post Service

Media Service

Image Processing Service

Video Processing Service

Comment Service

Reaction Service

Share Service

Feed Service

Recommendation Service

Group Service

Community Service

Page Service

Creator Service

Business Service

Event Service

Messaging Service

Presence Service

Notification Service

Search Service

Marketplace Service

Commerce Service

Payment Integration Service

Advertising Service

Analytics Service

Moderation Service

Spam Detection Service

Fraud Detection Service

Trust & Safety Service

Feature Flag Service

Audit Service

Administration Service

Developer Platform Service

AI Platform Gateway

────────────────────────────────────────

USER PROFILES

Design architecture supporting:

• Usernames

• Display Names

• Profile Photos

• Cover Photos

• Bios

• Personal Information

• Websites

• Professional Information

• Privacy Settings

• Profile Visibility

• Verification

• Account Recovery

• Account Deletion

• Memorialization readiness

• Multiple Account Types

• Profile Customization

All personal data must be designed with privacy controls and future data portability requirements in mind.

────────────────────────────────────────

SOCIAL GRAPH

Generate architecture for:

• Friend Requests

• Friend Acceptance

• Friend Removal

• Followers

• Following

• Follow Requests

• Suggested Connections

• Mutual Friends

• Relationship States

• Blocked Users

• Muted Users

• Restricted Users

• Privacy-aware Graph Queries

• High-volume Graph Reads

• Relationship Caching

• Graph Events

Optimize for hundreds of millions of users and extremely high read volumes.

────────────────────────────────────────

POSTS

Support:

• Text Posts

• Image Posts

• Video Posts

• Multi-media Posts

• Links

• Rich Link Previews

• Polls

• Check-ins

• Location Posts

• Shared Posts

• Reposts

• Collaborative Posts

• Scheduled Posts

• Drafts

• Public Posts

• Friends-only Posts

• Group Posts

• Page Posts

• Custom Audience Posts

• Edited Posts

• Deleted Posts

• Soft-deleted Content

────────────────────────────────────────

COMMENTS AND DISCUSSIONS

Generate architecture supporting:

• Comments

• Replies

• Nested Threads

• Comment Reactions

• Mentions

• Editing

• Deletion

• Moderation States

• Ranking

• Pagination

• Spam Detection

• Reporting

• High-volume Discussion Threads

────────────────────────────────────────

REACTIONS AND SHARING

Support:

• Likes

• Multiple Reaction Types

• Reaction Aggregates

• Idempotent Reactions

• Shares

• Reposts

• Quote Sharing

• Private Sharing

• Group Sharing

• External Sharing

• Engagement Events

• High-write-volume Counters

────────────────────────────────────────

NEWS FEED

Design a production-ready feed architecture supporting:

• Personalized Feed

• Friends Feed

• Following Feed

• Group Feed

• Page Feed

• Creator Feed

• Local Feed

• Trending Feed

• Recommended Feed

• Sponsored Feed

• Event-related Feed

Support:

• Candidate Generation

• Ranking

• Feed Filtering

• Privacy Enforcement

• Block Filtering

• Deduplication

• Cursor Pagination

• Feed Caching

• Fanout-on-write

• Fanout-on-read

• Hybrid Feed Strategies

• Feed Invalidation

• Experimentation

• Real-time Updates

Design the architecture so ranking systems and ML models can evolve independently from core feed delivery.

────────────────────────────────────────

GROUPS AND COMMUNITIES

Generate architecture supporting:

• Public Groups

• Private Groups

• Hidden Groups

• Communities

• Group Membership

• Membership Requests

• Invitations

• Roles

• Permissions

• Moderators

• Administrators

• Group Rules

• Group Posts

• Group Media

• Group Events

• Group Chat readiness

• Announcements

• Pinned Content

• Moderation Queues

• Member Management

────────────────────────────────────────

PAGES AND CREATOR PLATFORM

Support:

• Public Pages

• Creator Pages

• Business Pages

• Verification

• Followers

• Content Publishing

• Content Scheduling

• Team Members

• Role Management

• Analytics

• Audience Insights

• Content Insights

• Monetization readiness

• Brand Partnerships

• Creator Tools

────────────────────────────────────────

EVENTS

Generate architecture supporting:

• Event Creation

• Public Events

• Private Events

• Online Events

• Physical Events

• Hybrid Events

• Invitations

• RSVPs

• Guest Lists

• Event Discussions

• Event Media

• Event Notifications

• Calendar Integration

• Event Discovery

• Event Recommendations

• Ticketing Integration readiness

────────────────────────────────────────

MEDIA PLATFORM

Generate architecture supporting:

• Image Uploads

• Video Uploads

• Audio

• Documents where approved

• Albums

• Media Collections

• Profile Photos

• Cover Photos

• Group Media

• Event Media

• Page Media

• Marketplace Media

• Image Optimization

• Video Transcoding

• Thumbnail Generation

• Preview Generation

• Compression

• Metadata Extraction

• Malware Scanning

• Content Fingerprinting

• Signed Upload URLs

• Signed Download URLs

• CDN Delivery

• Lifecycle Policies

────────────────────────────────────────

MESSAGING

Design architecture supporting:

• One-to-One Conversations

• Group Conversations

• Community Messaging readiness

• Page-to-user Messaging

• Business Messaging

• Text Messages

• Images

• Videos

• Voice Messages

• Documents

• GIFs

• Stickers

• Emoji Reactions

• Typing Indicators

• Read Receipts

• Delivery States

• Presence

• Online Status

• Message Search

• Offline Synchronization

• Connection Recovery

• Multi-device Support

────────────────────────────────────────

VOICE AND VIDEO

Prepare architecture supporting:

• Voice Calls

• Video Calls

• Group Calls

• Screen Sharing

• WebRTC Signaling

• Call Notifications

• Call History

• Missed Calls

• Connection Quality Metrics

• Future Recording Support

────────────────────────────────────────

SEARCH

Design architecture for:

• User Search

• Page Search

• Creator Search

• Business Search

• Group Search

• Community Search

• Post Search

• Video Search

• Event Search

• Marketplace Search

• Location Search

• Hashtag Search

• Full-text Search

• Autocomplete

• Suggestions

• Typo Tolerance

• Filters

• Geo-aware Search

• Personalized Ranking

• Trending Searches

• Search Analytics

────────────────────────────────────────

MARKETPLACE

Generate architecture supporting:

• Product Listings

• Service Listings

• Categories

• Location-based Discovery

• Search

• Filters

• Seller Profiles

• Buyer Profiles

• Listing Media

• Saved Listings

• Messaging Between Buyers and Sellers

• Listing Moderation

• Reporting

• Availability

• Inventory readiness

• Payment Integration Boundaries

• Order Integration readiness

• Fraud Detection

────────────────────────────────────────

COMMERCE

Design service boundaries for:

• Product Catalogs

• Merchant Profiles

• Product Pages

• Shopping Content

• Inventory Integration

• Promotions

• Coupons

• Checkout Integration

• Payment Provider Integration

• Orders

• Order Tracking

• Refund Integration

Ensure commerce can evolve independently from the core social platform.

────────────────────────────────────────

NOTIFICATIONS

Generate architecture supporting:

• Push Notifications

• In-app Notifications

• Email Notifications

• Desktop Notifications

• SMS readiness

• Friend Requests

• Social Interactions

• Comments

• Reactions

• Mentions

• Shares

• Messages

• Group Activity

• Event Reminders

• Marketplace Activity

• Business Alerts

• Creator Alerts

• Notification Preferences

• Muting

• Aggregation

• Deduplication

────────────────────────────────────────

REAL-TIME FEATURES

Generate architecture for:

• WebSocket Authentication

• Connection Lifecycle

• Presence

• Typing Indicators

• Live Notifications

• Message Delivery

• Feed Update Readiness

• Call Signaling

• Heartbeats

• Connection Recovery

• Distributed Scaling

• Redis-backed Coordination

• Connection Metrics

────────────────────────────────────────

DATABASE ARCHITECTURE

Generate a complete PostgreSQL architecture.

Include:

• ERD

• Normalization Strategy

• Core Tables

• Foreign Keys

• Constraints

• Unique Indexes

• Composite Indexes

• Partial Indexes

• Partitioning Strategy

• Read Replica Strategy

• Archival Strategy

• Backup Strategy

• Global Replication Considerations

Optimize for:

• 1B+ users

• Hundreds of billions of relationships

• Billions of posts

• Billions of comments

• Billions of reactions

• Billions of media objects

• Extremely high read and write volumes

────────────────────────────────────────

END OF VOLUME 1

Continue architecture from this exact stopping point in:

Project 4 — Enterprise Facebook-Style Social Platform
Architecture Prompt — Volume 2

Do NOT begin backend implementation yet.
