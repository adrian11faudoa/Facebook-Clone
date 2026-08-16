Using the approved Project 4 — Enterprise Facebook-Style Social Platform Architecture Prompt — Volume 1, Architecture Prompt — Volume 2, Backend implementation, Backend Project Index, and the Master Prompt above.

Begin Frontend and Mobile implementation.

Do NOT redesign the approved architecture.

Do NOT redesign backend APIs, database ownership, event contracts, authentication architecture, authorization architecture, privacy architecture, or service boundaries.

Use the completed backend implementation and its API contracts as the source of truth.

If an API inconsistency or missing capability prevents correct frontend implementation:

1. Identify the exact issue.
2. Identify the affected frontend feature.
3. Propose the smallest backward-compatible correction.
4. Do not silently redesign the backend.

────────────────────────────────────────

MISSION

Build a production-ready, enterprise-scale social platform frontend.

Generate:

• Web Application
• Mobile Application
• Shared UI foundations where appropriate
• API clients
• Authentication flows
• Real-time integrations
• State management
• Caching
• Offline support where appropriate
• Accessibility
• Responsive design
• Error handling
• Loading states
• Empty states
• Optimistic updates
• Privacy-aware interfaces

The applications must be designed for millions of users and long-term product evolution.

Do not create a static mockup.

Implement real integrations with the completed backend.

────────────────────────────────────────

WEB TECHNOLOGY STACK

Use:

• Next.js
• React
• TypeScript
• Tailwind CSS

Use the architecture-approved versioning and project structure.

Apply:

• Strict TypeScript
• Feature-first organization
• Reusable components
• Accessible UI
• Responsive layouts
• Server/client boundaries where appropriate
• Secure API integration
• Production-ready error handling

────────────────────────────────────────

MOBILE TECHNOLOGY STACK

Use:

• React Native
• Expo
• TypeScript

Use:

• Expo Router or the architecture-approved navigation solution
• React Query or architecture-approved server-state management
• Zustand or architecture-approved client-state management

Support:

• iOS
• Android
• Push notifications
• Deep linking
• Offline-aware behavior
• Background synchronization where supported
• Secure token storage
• Media upload
• Real-time updates

────────────────────────────────────────

MONOREPO FRONTEND STRUCTURE

Implement the approved monorepo structure.

Maintain clear separation between:

apps/web/

apps/mobile/

packages/

Do not place web-specific code inside mobile applications.

Do not place mobile-specific code inside the web application.

Create shared packages only when they contain genuinely reusable:

• TypeScript types
• API contracts
• Validation utilities
• Design tokens
• Business-independent utilities
• Shared icons where appropriate

Do not move domain-specific UI logic into generic packages unnecessarily.

────────────────────────────────────────

DESIGN SYSTEM

Create a production-ready design system.

Include:

• Design tokens
• Typography
• Spacing
• Responsive breakpoints
• Layout primitives
• Colors
• Semantic colors
• Light mode
• Dark mode
• Elevation
• Borders
• Radius
• Motion guidelines
• Focus states
• Accessibility states

Generate reusable UI primitives including:

• Button
• IconButton
• Input
• Textarea
• Select
• Checkbox
• Radio
• Switch
• FormField
• Label
• Badge
• Avatar
• AvatarGroup
• Card
• Dialog
• Drawer
• Popover
• DropdownMenu
• Tooltip
• Tabs
• Pagination
• Skeleton
• Spinner
• Progress
• Toast
• Alert
• EmptyState
• ErrorState
• LoadingState

Do not build every page with duplicated components.

────────────────────────────────────────

ACCESSIBILITY

Implement accessibility as a core requirement.

Support:

• Semantic HTML
• Keyboard navigation
• Visible focus management
• Screen readers
• Accessible forms
• Accessible dialogs
• ARIA where appropriate
• Color contrast
• Reduced motion
• Accessible error messages
• Accessible notifications
• Accessible media controls

For mobile:

• Accessibility labels
• Accessibility roles
• Screen-reader compatibility
• Sufficient touch target sizes

────────────────────────────────────────

APPLICATION SHELL

Implement the core application shell.

Web must support:

• Responsive top navigation
• Left navigation
• Main content area
• Optional right sidebar
• Mobile responsive navigation
• Global search access
• Notifications
• Messaging access
• Account menu

Mobile must support appropriate navigation for:

• Home
• Search/Discover
• Create
• Notifications
• Profile

Use platform-appropriate navigation patterns.

────────────────────────────────────────

AUTHENTICATION UI

Implement complete authentication experiences.

Support:

• Registration
• Login
• Logout
• Email verification
• Password reset
• Password change
• OAuth
• Multi-factor authentication
• Recovery codes
• Passkey support where backend support exists
• Session management
• Device management
• Security notifications
• Account recovery

Implement:

• Form validation
• Server error handling
• Rate-limit feedback
• Loading states
• Secure token handling
• Session expiration handling
• Automatic refresh where appropriate

Never expose sensitive authentication details unnecessarily.

────────────────────────────────────────

ONBOARDING

Implement onboarding supporting:

• Profile setup
• Username selection
• Profile photo
• Bio
• Privacy preferences
• Interest selection where approved
• Friend discovery
• Contact discovery permission flow
• Notification permissions
• Optional personalization setup

Onboarding must be resumable.

────────────────────────────────────────

HOME AND NEWS FEED

Implement the primary social feed.

Support:

• Personalized feed
• Friends feed
• Following feed
• Group feed
• Community feed
• Page feed
• Creator content
• Recommended content
• Trending content
• Sponsored-content boundaries

Implement:

• Cursor pagination
• Infinite scrolling
• Pull-to-refresh on mobile
• Loading skeletons
• Empty states
• Retry behavior
• Optimistic interactions
• Cache invalidation
• Privacy-aware rendering
• Content deduplication on the client where needed

Do not allow client-side state to become the authoritative source of feed consistency.

────────────────────────────────────────

POST COMPOSER

Implement a production-ready content creation experience.

Support:

• Text
• Images
• Videos
• Multiple media attachments
• Link sharing
• Polls
• Check-ins
• Location
• Mentions
• Hashtags
• Audience selection
• Scheduling where approved
• Drafts where approved

Implement:

• Validation
• Media previews
• Upload progress
• Upload retry
• Cancellation
• Processing states
• Failed upload recovery
• Optimistic publishing where safe

Use backend-provided signed upload flows where implemented.

Do not route large uploads through frontend application servers.

────────────────────────────────────────

POST EXPERIENCE

Implement reusable post components.

Support:

• Author information
• Visibility indicators
• Text
• Rich text
• Media
• Link previews
• Polls
• Location
• Engagement counts
• Reactions
• Comments
• Shares
• Save actions
• Report actions
• Edit
• Delete

Respect:

• Authorization
• Privacy
• Moderation state
• Deleted content behavior

────────────────────────────────────────

COMMENTS

Implement:

• Comment lists
• Nested replies
• Create comment
• Edit comment
• Delete comment
• Reactions
• Mentions
• Pagination
• Loading states
• Error recovery
• Optimistic updates where safe
• Reporting

Support mobile-friendly interaction patterns.

────────────────────────────────────────

REACTIONS

Implement:

• Reaction picker
• Add reaction
• Change reaction
• Remove reaction
• Reaction summaries
• User lists where authorized

Use optimistic updates with rollback behavior.

────────────────────────────────────────

SOCIAL GRAPH

Implement interfaces for:

• Friend requests
• Accept
• Decline
• Cancel request
• Remove friend
• Follow
• Unfollow
• Follow requests where applicable
• Mutual connections
• Suggested connections
• Block
• Unblock
• Mute
• Restrict

Every action must reflect backend authorization and privacy rules.

────────────────────────────────────────

PROFILE

Implement complete profile experiences.

Support:

• Profile header
• Avatar
• Cover image
• Bio
• Profile details
• Posts
• Media
• Friends
• Followers
• Following
• Groups
• Events
• Marketplace activity where permitted
• Privacy settings
• Edit profile

Implement privacy-aware rendering based on backend data.

Do not infer visibility rules exclusively on the client.

────────────────────────────────────────

GROUPS AND COMMUNITIES

Implement:

• Group discovery
• Group profiles
• Membership
• Membership requests
• Invitations
• Group feed
• Rules
• Announcements
• Pinned content
• Member lists where permitted
• Administration interfaces
• Moderation interfaces where authorized

Implement separate community experiences where defined by the backend architecture.

────────────────────────────────────────

PAGES

Implement:

• Public pages
• Creator pages
• Business pages
• Page profiles
• Page content
• Followers
• Page management
• Team member management where authorized
• Page analytics dashboards where available

────────────────────────────────────────

CREATOR EXPERIENCE

Implement creator-focused interfaces.

Support:

• Creator profile
• Audience metrics
• Content performance
• Engagement metrics
• Growth metrics
• Creator settings
• Monetization readiness interfaces

Do not expose analytics beyond the user's authorization level.

────────────────────────────────────────

BUSINESS EXPERIENCE

Implement:

• Business profiles
• Business settings
• Team management
• Verification status
• Content management
• Analytics
• Commerce boundaries

────────────────────────────────────────

EVENTS

Implement:

• Event discovery
• Event details
• Event creation
• Event editing
• RSVP
• Guest lists where authorized
• Invitations
• Event discussions
• Event media
• Event reminders
• Online event metadata
• Physical location information

────────────────────────────────────────

MESSAGING

Implement real-time messaging.

Support:

• Conversation list
• One-to-one conversations
• Group conversations
• Page messaging
• Business messaging
• Message creation
• Text messages
• Media messages
• Replies
• Reactions
• Read receipts
• Delivery states
• Typing indicators
• Conversation pagination
• Offline-aware states
• Connection recovery
• Multi-device synchronization behavior

Implement:

• Real-time Socket.IO integration
• Optimistic message sending
• Retry behavior
• Failed message states
• Duplicate prevention
• Reconnection handling

Follow the approved privacy and encryption architecture.

────────────────────────────────────────

NOTIFICATIONS

Implement:

• Notification center
• Notification grouping
• Read state
• Notification preferences
• Muting
• Deep linking
• Real-time updates
• Push notification handling on mobile

Support graceful fallback when real-time connectivity is unavailable.

────────────────────────────────────────

SEARCH AND DISCOVERY

Implement search experiences for:

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

Support:

• Autocomplete
• Search suggestions
• Filters
• Recent searches where appropriate
• Infinite pagination
• Loading states
• Empty states
• Error states

────────────────────────────────────────

MARKETPLACE

Implement:

• Marketplace home
• Categories
• Listing discovery
• Search
• Filters
• Listing details
• Seller profiles
• Listing creation
• Listing editing
• Saved listings
• Availability states
• Buyer-seller messaging
• Reporting
• Safety indicators

────────────────────────────────────────

COMMERCE

Implement approved commerce interfaces.

Support:

• Product catalogs
• Product details
• Merchant profiles
• Promotions
• Coupons
• Cart boundaries where approved
• Checkout integration boundaries
• Orders
• Order history
• Order status

Never trust client-side payment state.

────────────────────────────────────────

ADVERTISING MANAGEMENT

Implement authorized advertising interfaces.

Support:

• Advertising organizations
• Ad accounts
• Campaigns
• Ad sets
• Ads
• Creative assets
• Targeting configuration
• Budgets
• Scheduling
• Campaign status
• Review status
• Experimentation
• Reporting

Create clear interfaces for advertiser roles and permissions.

────────────────────────────────────────

AD DELIVERY UI

Implement sponsored content presentation.

Requirements:

• Clearly distinguish sponsored content where required.
• Respect privacy and personalization controls.
• Handle unavailable advertisements gracefully.
• Do not make feed rendering dependent on advertising success.

────────────────────────────────────────

MODERATION INTERFACES

Implement authorized moderation tools.

Support:

• Moderation queues
• Report details
• Evidence references
• Content review
• User review
• Decisions
• Enforcement actions
• Moderator notes
• Appeals
• Audit visibility where authorized

Do not expose moderator tools to unauthorized users.

────────────────────────────────────────

ADMINISTRATION

Implement administrative interfaces where approved.

Support:

• User management
• Content management
• Group and community management
• Page and business management
• Marketplace administration
• Advertising administration
• Feature flags
• System health summaries
• Audit logs where authorized

Keep administrative interfaces isolated from standard user interfaces.

────────────────────────────────────────

FEATURE FLAGS

Integrate the backend feature flag architecture.

Support:

• Server-provided flags
• Safe client-side evaluation where approved
• Default values
• Kill switches
• Feature rollout
• Experiment assignments

The application must fail safely when the feature flag service is unavailable.

────────────────────────────────────────

ANALYTICS UI

Implement dashboards appropriate to authorized roles.

Support:

• Creator analytics
• Business analytics
• Marketplace analytics
• Advertising analytics
• Administrative analytics

Use:

• Date ranges
• Filters
• Loading states
• Empty states
• Error states

Do not expose raw analytics data unnecessarily.

────────────────────────────────────────

AI FEATURES

Integrate only the AI capabilities approved by the backend.

Support interfaces for applicable features such as:

• Content assistance
• Translation
• Accessibility descriptions
• Search assistance
• Summarization
• Creator assistance
• Business assistance

Implement:

• Loading states
• Failure handling
• Usage limits
• Safety messaging
• Privacy-aware controls

Do not expose provider-specific implementation details to users.

────────────────────────────────────────

PRIVACY AND SAFETY SETTINGS

Implement comprehensive settings for:

• Profile privacy
• Audience defaults
• Post visibility
• Friend visibility
• Follower visibility
• Search visibility
• Location privacy
• Contact discovery
• Messaging permissions
• Blocking
• Muting
• Restricting
• Notification preferences
• Advertising preferences
• Personalization
• Analytics consent
• AI data controls
• Data export
• Account deletion

Every setting must integrate with the backend as the source of truth.

────────────────────────────────────────

SETTINGS

Implement:

• Account settings
• Security settings
• Privacy settings
• Notification settings
• Appearance
• Accessibility preferences
• Language
• Device management
• Connected applications
• Data management

Support light and dark mode.

────────────────────────────────────────

API CLIENT ARCHITECTURE

Generate a production-ready API layer.

Support:

• Typed requests
• Typed responses
• Authentication
• Token refresh
• Request cancellation
• Error normalization
• Request correlation
• Retry behavior where safe
• Pagination helpers
• Upload support
• WebSocket integration

Do not duplicate API contracts manually when shared generated or typed contracts are available.

────────────────────────────────────────

STATE MANAGEMENT

Separate state appropriately.

Use server-state management for:

• API data
• Caching
• Revalidation
• Pagination
• Mutations

Use client-state management only for appropriate concerns such as:

• UI state
• Temporary drafts
• Local preferences
• Navigation state where needed

Do not place all application state in a single global store.

────────────────────────────────────────

OFFLINE SUPPORT

For mobile, implement offline-aware behavior where appropriate.

Support:

• Cached content
• Offline indicators
• Retry queues where approved
• Draft persistence
• Message state awareness
• Network recovery

Do not pretend an action succeeded when it has not been accepted by the backend.

────────────────────────────────────────

ERROR HANDLING

Implement:

• Application-level error boundaries
• Route-level error handling
• API error handling
• Form errors
• Network failure handling
• Authentication failure handling
• Permission failure handling
• Not found states
• Retry actions

Never expose internal backend details directly to users.

────────────────────────────────────────

PERFORMANCE

Optimize for:

• Code splitting
• Lazy loading
• Image optimization
• Video optimization
• Virtualized lists
• Feed rendering
• Memory efficiency
• Bundle size
• Cache efficiency
• Mobile performance

Measure before introducing unnecessary optimization complexity.

────────────────────────────────────────

TESTING

Generate tests continuously.

Include:

Web:

• Component tests
• Hook tests
• Integration tests
• Accessibility tests
• API client tests
• End-to-end tests

Mobile:

• Component tests
• Navigation tests
• State tests
• API integration tests
• Offline behavior tests
• Deep-link tests

Generate tests as features are implemented.

────────────────────────────────────────

IMPLEMENTATION ORDER

Implement incrementally in the following approximate order.

Milestone Group 1

• Frontend monorepo foundation
• Shared packages
• Design system
• API client
• Authentication foundation
• State management
• Error handling
• Application shells

Milestone Group 2

• Authentication
• Onboarding
• Session management
• Settings foundation

Milestone Group 3

• Profiles
• Social graph
• Friends
• Followers
• Privacy controls

Milestone Group 4

• Post composer
• Media uploads
• Posts
• Comments
• Reactions
• Sharing

Milestone Group 5

• Home
• Feed
• Feed interactions
• Recommendations

Milestone Group 6

• Groups
• Communities
• Pages
• Creators
• Businesses
• Events

Milestone Group 7

• Messaging
• WebSocket integration
• Presence
• Notifications

Milestone Group 8

• Search
• Discovery
• Marketplace
• Commerce

Milestone Group 9

• Advertising management
• Sponsored content
• Analytics dashboards

Milestone Group 10

• Moderation
• Administration
• Feature flags
• AI integrations

Milestone Group 11

• Offline behavior
• Performance optimization
• Accessibility validation
• Security validation
• End-to-end testing
• Production hardening

────────────────────────────────────────

PROJECT INDEX

Maintain a living Frontend Project Index.

After every milestone update:

• Current milestone
• Completed web features
• Completed mobile features
• Generated files
• API integrations
• WebSocket integrations
• State management modules
• Shared components
• Test coverage
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

Implement incrementally.

Each milestone should contain approximately 20–40 files.

At the end of every milestone:

1. Verify compilation consistency.
2. Verify backend API compatibility.
3. Verify authentication and authorization integration.
4. Verify privacy behavior.
5. Verify accessibility for completed features.
6. Verify responsive behavior where applicable.
7. Update the Frontend Project Index.
8. List completed features.
9. Identify the exact next file or implementation unit.

STOP.

Wait for approval before generating the next milestone.

The next prompt after frontend implementation will be:

Project 4 — Enterprise Facebook-Style Social Platform
Infrastructure Prompt
