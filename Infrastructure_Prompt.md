Using the approved Project 4 — Enterprise Facebook-Style Social Platform Architecture Prompt — Volume 1, Architecture Prompt — Volume 2, completed Backend implementation, completed Frontend and Mobile implementation, all Project Indexes, and the Master Prompt above.

Begin Infrastructure, DevOps, CI/CD, Observability, Testing Infrastructure, Deployment, and Production Hardening implementation.

Do NOT redesign the approved application architecture.

Do NOT redesign:

• Service boundaries
• Database ownership
• API contracts
• Event contracts
• Authentication architecture
• Authorization architecture
• Privacy architecture
• Backend architecture
• Frontend architecture

The approved architecture and completed implementations are the source of truth.

If an infrastructure issue requires an application-level modification:

1. Identify the exact issue.
2. Identify the affected service or application.
3. Explain why the modification is required.
4. Propose the smallest backward-compatible change.
5. Do not silently redesign the application.

────────────────────────────────────────

MISSION

Build a production-ready, secure, scalable, observable, and deployable infrastructure platform for the Enterprise Facebook-Style Social Platform.

The infrastructure must support:

• Global deployment
• Multi-region readiness
• Horizontal scaling
• High availability
• Zero-downtime deployments
• Secure secret management
• Automated CI/CD
• Infrastructure as Code
• Database reliability
• Backup and recovery
• Distributed caching
• Event streaming
• Background processing
• Search infrastructure
• Object storage
• CDN delivery
• WebSocket scaling
• Monitoring
• Logging
• Distributed tracing
• Alerting
• Security monitoring
• Disaster recovery
• Performance testing
• Production hardening

Design and implement infrastructure suitable for a platform capable of supporting millions of active users and future global expansion.

────────────────────────────────────────

INFRASTRUCTURE TECHNOLOGY STACK

Use the architecture-approved technologies.

Primary infrastructure technologies:

• Docker
• Docker Compose
• Kubernetes
• Helm
• Terraform
• GitHub Actions
• PostgreSQL
• Redis
• Kafka or Redpanda
• BullMQ
• Elasticsearch or OpenSearch
• S3-compatible object storage
• CloudFront or approved CDN
• Prometheus
• Grafana
• Loki
• Tempo
• OpenTelemetry
• HashiCorp Vault or approved secrets architecture

Do not introduce unnecessary infrastructure technologies.

────────────────────────────────────────

IMPLEMENTATION PRINCIPLES

Apply:

• Infrastructure as Code
• Immutable infrastructure where practical
• Declarative configuration
• Least privilege
• Defense in depth
• Environment isolation
• Secret isolation
• Idempotent deployments
• Automated validation
• Automated rollback readiness
• Horizontal scalability
• Failure isolation
• Observability by default
• Secure defaults
• Cost awareness
• Disaster recovery readiness

Do not rely on undocumented manual production steps.

Every production dependency must have a defined deployment and operational strategy.

────────────────────────────────────────

INFRASTRUCTURE DIRECTORY STRUCTURE

Implement the approved infrastructure structure.

Organize infrastructure clearly, for example:

infrastructure/

  docker/

  compose/

  kubernetes/

  helm/

  terraform/

  environments/

  monitoring/

  observability/

  security/

  scripts/

  backups/

  disaster-recovery/

  load-testing/

  ci/

docs/

  infrastructure/

  runbooks/

  architecture/

Do not place production secrets inside the repository.

────────────────────────────────────────

ENVIRONMENTS

Create infrastructure support for:

• Local
• Development
• Staging
• Production

Each environment must have:

• Independent configuration
• Environment-specific variables
• Separate secrets
• Appropriate scaling
• Appropriate monitoring
• Environment-specific resource limits
• Deployment policies

Production configuration must never be used by local development.

────────────────────────────────────────

DOCKER IMPLEMENTATION

Generate production-ready Dockerfiles for:

• API Gateway
• Authentication Service
• Authorization Service
• Identity Service
• User Service
• Profile Service
• Social Graph Service
• Post Service
• Media Service
• Feed Service
• Recommendation Service
• Group Service
• Community Service
• Page Service
• Creator Service
• Business Service
• Event Service
• Messaging Service
• Presence Service
• Notification Service
• Search Service
• Marketplace Service
• Commerce Service
• Payment Integration Service
• Advertising Service
• Ad Delivery Service
• Analytics Service
• Moderation Service
• Trust & Safety Service
• Feature Flag Service
• Audit Service
• Developer Platform Service
• AI Platform Gateway

Also generate Dockerfiles for:

• Web application
• Mobile build infrastructure where appropriate
• Background workers
• Media processing workers

Use:

• Multi-stage builds
• Minimal production images
• Non-root users
• Explicit dependency installation
• Production-only dependencies where appropriate
• Health checks where applicable
• Reproducible builds

Do not use development images in production.

────────────────────────────────────────

DOCKER COMPOSE

Generate Docker Compose infrastructure for local development.

Support local instances of:

• PostgreSQL
• Redis
• Kafka or Redpanda
• Elasticsearch or OpenSearch
• Object storage emulator or S3-compatible service
• Required backend services
• Background workers
• Web application
• Observability services where practical

Include:

• Named volumes
• Health checks
• Dependency conditions
• Environment variables
• Local networking
• Service profiles where useful
• Development overrides

Local development must be easy to start and stop.

────────────────────────────────────────

KUBERNETES ARCHITECTURE

Generate production-ready Kubernetes manifests or Helm-based infrastructure.

Support:

• Namespaces
• Deployments
• StatefulSets where required
• Services
• ConfigMaps
• Secret references
• ServiceAccounts
• RBAC
• NetworkPolicies
• PersistentVolumeClaims
• Ingress
• HorizontalPodAutoscalers
• PodDisruptionBudgets
• Resource requests
• Resource limits
• Liveness probes
• Readiness probes
• Startup probes
• Affinity and anti-affinity where appropriate
• Topology spread constraints
• Autoscaling

Separate workloads by responsibility.

────────────────────────────────────────

KUBERNETES NAMESPACES

Design appropriate namespace boundaries such as:

• platform-system
• application
• workers
• data
• observability
• monitoring
• security
• ingress

Do not create namespaces without clear operational value.

────────────────────────────────────────

HELM

Generate Helm charts for:

• Shared application deployment patterns
• Individual services where justified
• Web application
• Worker deployments
• Observability components
• Environment-specific values

Support:

• Development values
• Staging values
• Production values

Avoid duplicated Kubernetes YAML when reusable Helm templates are appropriate.

Do not hide critical configuration inside overly complex templates.

────────────────────────────────────────

SERVICE DEPLOYMENT STANDARD

Every backend service deployment must support:

• Replica configuration
• Environment configuration
• Secret injection
• Resource requests
• Resource limits
• Liveness probes
• Readiness probes
• Startup probes
• Graceful termination
• Horizontal scaling
• Pod disruption protection
• Structured logging
• OpenTelemetry configuration

Every worker deployment must support:

• Configurable concurrency
• Resource limits
• Graceful shutdown
• Retry compatibility
• Queue connection configuration
• Health monitoring

────────────────────────────────────────

API GATEWAY DEPLOYMENT

Implement infrastructure supporting:

• External ingress
• TLS termination
• Rate limiting boundaries
• Request size limits
• Timeout configuration
• Health checks
• Load balancing
• DDoS protection integration boundaries
• WAF readiness
• Horizontal scaling

Do not expose internal services unnecessarily to the public internet.

────────────────────────────────────────

WEB APPLICATION DEPLOYMENT

Implement production deployment for the Next.js application.

Support:

• Optimized production builds
• Environment configuration
• CDN integration boundaries
• Caching strategy
• Static asset delivery
• Image optimization
• Health checks
• Horizontal scaling
• Zero-downtime deployments

────────────────────────────────────────

MOBILE APPLICATION INFRASTRUCTURE

Create CI/CD support for:

• Android builds
• iOS builds
• Development builds
• Staging builds
• Production builds

Support:

• Environment configuration
• Secure signing credential handling
• Build validation
• Version management
• Release readiness

Do not commit signing credentials to the repository.

────────────────────────────────────────

POSTGRESQL INFRASTRUCTURE

Implement the approved PostgreSQL deployment architecture.

Support:

• Production database provisioning
• High availability readiness
• Primary database
• Read replicas where approved
• Connection pooling
• Backup automation
• Point-in-time recovery readiness
• Encryption
• Monitoring
• Slow query monitoring
• Connection monitoring
• Disk monitoring
• Replication monitoring
• Migration strategy

Define:

• Backup schedules
• Retention policies
• Restore procedures
• Disaster recovery procedures

Prisma migrations must be integrated safely into deployment workflows.

Do not allow uncontrolled concurrent migration execution.

────────────────────────────────────────

DATABASE MIGRATIONS

Implement a safe migration process.

Support:

• Migration validation
• Staging validation
• Controlled production execution
• Backward-compatible migrations
• Expand-and-contract patterns where required
• Roll-forward strategy
• Migration observability

Never depend on destructive production migrations without explicit safety procedures.

────────────────────────────────────────

REDIS INFRASTRUCTURE

Deploy Redis for approved workloads.

Support:

• Caching
• Sessions
• Rate limiting
• Distributed coordination
• Presence
• WebSocket scaling
• BullMQ

Define:

• High availability strategy
• Persistence where required
• Eviction policies
• Memory monitoring
• Connection limits
• Failure behavior
• Backup requirements

Do not allow cache failure to cause unnecessary total platform failure.

────────────────────────────────────────

KAFKA OR REDPANDA INFRASTRUCTURE

Deploy the approved event backbone.

Support:

• Multiple brokers
• Topic configuration
• Replication
• Partitioning
• Retention
• Consumer groups
• Dead-letter topics
• Monitoring
• Security
• Authentication
• Authorization
• Encryption

Define:

• Production topic configuration
• Replication factors
• Partition scaling strategy
• Retention policies
• Recovery procedures
• Schema compatibility

Event infrastructure must support high-volume asynchronous workloads.

────────────────────────────────────────

BULLMQ INFRASTRUCTURE

Deploy infrastructure supporting:

• Queue workers
• Horizontal worker scaling
• Concurrency control
• Retry processing
• Delayed jobs
• Scheduled jobs
• Dead-letter workflows
• Queue monitoring

Separate resource-intensive workers from latency-sensitive API services.

────────────────────────────────────────

SEARCH INFRASTRUCTURE

Deploy Elasticsearch or OpenSearch.

Support:

• Cluster configuration
• Index lifecycle management
• Replicas
• Snapshots
• Monitoring
• Access controls
• TLS
• Index scaling
• Reindexing procedures
• Capacity monitoring

Support the approved indexes for:

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

────────────────────────────────────────

OBJECT STORAGE

Implement S3-compatible storage architecture.

Support separate storage prefixes or buckets for:

• Profile media
• Cover media
• Post images
• Post videos
• Group media
• Community media
• Page media
• Business media
• Marketplace media
• Advertising assets
• Temporary uploads
• Processed media
• Thumbnails
• Moderation evidence where authorized

Implement:

• IAM isolation
• Signed URLs
• Lifecycle policies
• Encryption
• Access controls
• Retention
• CDN integration
• Replication readiness

────────────────────────────────────────

CDN

Implement CDN architecture for:

• Images
• Videos
• Static web assets
• Media previews
• Thumbnails

Support:

• Cache policies
• Origin access restrictions
• Signed delivery where required
• Cache invalidation
• Geographic distribution
• Security headers
• DDoS mitigation boundaries

Do not expose object storage publicly when controlled delivery is required.

────────────────────────────────────────

MEDIA PROCESSING INFRASTRUCTURE

Deploy workers for:

• Image processing
• Video transcoding
• Thumbnail generation
• Preview generation
• Metadata extraction
• Media cleanup

Support:

• Resource isolation
• CPU-intensive workloads
• Horizontal scaling
• Queue-based execution
• Retry handling
• Timeout handling
• Failure recovery

Do not allow media processing workloads to starve core API services.

────────────────────────────────────────

WEBSOCKET INFRASTRUCTURE

Deploy real-time infrastructure supporting:

• Socket.IO
• Horizontal scaling
• Redis coordination
• Connection routing
• Load balancing
• Sticky sessions only if required by the selected scaling model
• Connection limits
• Heartbeat configuration
• Graceful connection draining
• Metrics

Support:

• Messaging
• Presence
• Typing indicators
• Notifications
• Live updates
• WebRTC signaling

────────────────────────────────────────

INGRESS AND NETWORKING

Implement secure networking.

Support:

• Ingress controller
• TLS
• HTTPS-only public access
• Internal services
• NetworkPolicies
• Service-to-service isolation
• Private data services
• Public API boundaries

Define:

• Public services
• Private services
• Internal-only services
• Data-plane boundaries
• Administrative access boundaries

────────────────────────────────────────

TLS AND CERTIFICATE MANAGEMENT

Implement:

• Automated certificate provisioning where appropriate
• Certificate renewal
• HTTPS enforcement
• Secure TLS configuration

Support internal encryption where required by the security architecture.

────────────────────────────────────────

SECRETS MANAGEMENT

Implement the approved secrets architecture.

Use HashiCorp Vault or the architecture-approved equivalent.

Support secrets for:

• Database credentials
• Redis credentials
• Kafka credentials
• Object storage
• OAuth credentials
• Email providers
• Push notification providers
• Payment providers
• AI providers
• Monitoring services
• Application secrets
• Encryption keys

Implement:

• Secret rotation readiness
• Access policies
• Kubernetes integration
• Audit logging
• Least privilege

Never commit secrets to source control.

────────────────────────────────────────

KUBERNETES SECURITY

Implement:

• ServiceAccounts
• RBAC
• Least privilege
• NetworkPolicies
• Non-root containers
• Read-only filesystems where practical
• Security contexts
• Resource limits
• Image security policies where supported
• Secret isolation

────────────────────────────────────────

CONTAINER SECURITY

Implement security practices supporting:

• Dependency scanning
• Container image scanning
• Base image update strategy
• Vulnerability detection
• Image provenance where available
• Non-root execution
• Minimal images
• Production dependency isolation

────────────────────────────────────────

TERRAFORM

Generate Terraform infrastructure for the approved cloud architecture.

Organize reusable modules for:

• Networking
• VPC or equivalent
• Subnets
• Routing
• Kubernetes
• Container registry
• PostgreSQL
• Redis
• Kafka or managed equivalent
• Search
• Object storage
• CDN
• DNS
• IAM
• Secrets
• Monitoring
• Backups

Support separate environments.

Use:

• Remote state
• State locking
• Environment isolation
• Reusable modules
• Explicit dependencies
• Tagging strategy

Do not hardcode credentials.

────────────────────────────────────────

CLOUD ARCHITECTURE

Design production infrastructure supporting:

• Multiple availability zones
• Private networking for internal workloads
• Public entry points only where required
• Managed services where architecturally appropriate
• Horizontal scaling
• Backup infrastructure
• Monitoring
• Disaster recovery

Do not unnecessarily couple the entire infrastructure to a single cloud provider when abstractions are practical.

────────────────────────────────────────

CI/CD WITH GITHUB ACTIONS

Implement pipelines for:

• Pull request validation
• Type checking
• Linting
• Unit tests
• Integration tests
• Contract tests
• Security scanning
• Dependency scanning
• Container builds
• Container scanning
• Build artifact generation

Support deployment pipelines for:

• Development
• Staging
• Production

Production deployment must include:

• Approval boundaries where appropriate
• Migration control
• Health validation
• Rollback readiness
• Deployment notifications

────────────────────────────────────────

CI PIPELINE

On every relevant pull request:

1. Install dependencies.
2. Validate dependency integrity.
3. Run formatting checks.
4. Run linting.
5. Run TypeScript validation.
6. Run unit tests.
7. Run integration tests where practical.
8. Run contract tests.
9. Run security checks.
10. Build applications.
11. Build containers.
12. Scan containers.
13. Publish test reports.

Fail fast where appropriate.

────────────────────────────────────────

CD PIPELINE

Implement controlled deployment flow:

Development:

• Automatic deployment after approved merge.

Staging:

• Automated deployment.
• Integration validation.
• Smoke tests.

Production:

• Build promotion.
• Environment validation.
• Migration validation.
• Controlled rollout.
• Health checks.
• Metrics validation.
• Rollback readiness.

Never rebuild different artifacts independently for every environment when artifact promotion is possible.

────────────────────────────────────────

DEPLOYMENT STRATEGIES

Support readiness for:

• Rolling deployments
• Canary deployments
• Blue-green deployments

Use the simplest deployment strategy appropriate to the service.

Support:

• Health validation
• Error-rate monitoring
• Latency monitoring
• Automated or operator-assisted rollback

────────────────────────────────────────

OBSERVABILITY

Implement a complete observability stack.

Use:

• OpenTelemetry
• Prometheus
• Grafana
• Loki
• Tempo

Support:

Metrics:

• HTTP requests
• Latency
• Error rates
• Database performance
• Redis performance
• Kafka health
• Queue health
• Search health
• WebSocket connections
• Media processing
• Resource utilization
• Business metrics

Logs:

• Structured logging
• Centralized collection
• Correlation IDs
• Request IDs
• Trace IDs
• Privacy-aware logging

Tracing:

• HTTP requests
• Internal service communication
• Database operations
• Redis operations
• Kafka events
• BullMQ jobs
• WebSocket flows

────────────────────────────────────────

PROMETHEUS

Configure monitoring for:

• Kubernetes
• Nodes
• Pods
• Services
• PostgreSQL
• Redis
• Kafka or Redpanda
• Elasticsearch or OpenSearch
• Application services
• Workers

Generate appropriate scrape configurations and alert rules.

────────────────────────────────────────

GRAFANA

Create dashboards for:

• Platform overview
• API Gateway
• Backend services
• PostgreSQL
• Redis
• Kafka or Redpanda
• Queues
• Search
• WebSockets
• Media processing
• Kubernetes
• Business metrics

Dashboards must help operators diagnose failures quickly.

────────────────────────────────────────

LOKI

Implement centralized logging.

Support:

• Structured log ingestion
• Service labels
• Environment labels
• Trace correlation
• Retention policies
• Access controls

Avoid logging:

• Passwords
• Tokens
• Secrets
• Sensitive personal data unless explicitly required and protected

────────────────────────────────────────

TEMPO AND DISTRIBUTED TRACING

Implement distributed tracing.

Support trace propagation across:

• API Gateway
• Backend services
• Database operations
• Redis
• Kafka
• BullMQ
• WebSocket flows

────────────────────────────────────────

ALERTING

Define alerts for:

Critical:

• API unavailable
• Database unavailable
• Regional failure
• Kafka failure
• Search cluster failure
• Authentication failure spike
• Severe error-rate spike
• Security incident indicators

Warning:

• High latency
• Increasing error rate
• Database connection pressure
• Redis memory pressure
• Queue backlog
• Kafka consumer lag
• Search pressure
• Disk pressure
• High CPU
• High memory

Every critical alert must have an associated runbook.

────────────────────────────────────────

SLOs AND ERROR BUDGETS

Define initial SLIs and SLOs for:

• API availability
• API latency
• Authentication success
• Feed delivery
• Messaging delivery
• Notification delivery
• Search availability
• Media upload availability
• Background processing

Define error-budget policies for deployment and reliability decisions.

────────────────────────────────────────

BACKUPS

Implement automated backups for:

• PostgreSQL
• Search indexes where required
• Configuration
• Critical metadata
• Secrets configuration references where applicable

Support:

• Backup schedules
• Retention
• Encryption
• Cross-region readiness
• Restore testing

A backup strategy without tested restore procedures is incomplete.

────────────────────────────────────────

DISASTER RECOVERY

Implement operational readiness for:

• Service failure
• Pod failure
• Node failure
• Availability zone failure
• Database failure
• Redis failure
• Kafka failure
• Search failure
• Kubernetes failure
• Object storage failure
• CDN failure
• DNS failure
• Regional failure
• Secret management failure
• Security incidents

For each critical scenario define:

• Detection
• Immediate mitigation
• Failover procedure
• Recovery procedure
• Data validation
• Failback procedure

────────────────────────────────────────

DISASTER RECOVERY RUNBOOKS

Generate runbooks for:

• Database restore
• Database failover
• Redis recovery
• Kafka recovery
• Search recovery
• Kubernetes cluster failure
• Service rollback
• Failed deployment
• Secret rotation
• Compromised credential
• Regional outage
• Data corruption
• Queue backlog
• Consumer lag
• Object storage failure

────────────────────────────────────────

LOAD TESTING

Create performance and load-testing infrastructure.

Support testing for:

• Authentication
• Feed retrieval
• Post creation
• Comments
• Reactions
• Messaging
• Notifications
• Search
• Marketplace
• WebSocket connections

Generate realistic scenarios for:

• Normal load
• Peak load
• Stress testing
• Spike testing
• Soak testing

Do not run destructive load tests against production without explicit safeguards.

────────────────────────────────────────

SECURITY TESTING

Integrate:

• Dependency scanning
• Static analysis
• Secret scanning
• Container scanning
• Infrastructure scanning
• API security testing readiness

Implement automated checks where practical.

────────────────────────────────────────

PRODUCTION HARDENING

Before completing the infrastructure phase, validate:

• No secrets are committed.
• Production containers run as non-root.
• Resource limits are configured.
• Health checks exist.
• Services shut down gracefully.
• Database backups are configured.
• Restore procedures exist.
• Monitoring is operational.
• Logging is centralized.
• Distributed tracing is operational.
• Alerts are configured.
• Critical runbooks exist.
• CI/CD pipelines validate builds.
• Production deployment supports rollback.
• Network boundaries are defined.
• Least privilege is applied.
• Infrastructure is reproducible using Terraform.
• Kubernetes configuration supports high availability.

────────────────────────────────────────

DOCUMENTATION

Generate infrastructure documentation covering:

• Local development setup
• Environment architecture
• Deployment process
• CI/CD pipelines
• Terraform usage
• Kubernetes operations
• Monitoring
• Logging
• Tracing
• Alert response
• Backup and restore
• Disaster recovery
• Security operations
• Scaling procedures

────────────────────────────────────────

IMPLEMENTATION ORDER

Implement incrementally in the following approximate order.

Milestone Group 1

• Infrastructure directory foundation
• Environment configuration
• Docker foundation
• Docker Compose
• Shared infrastructure scripts

Milestone Group 2

• Terraform foundation
• Networking
• IAM
• Kubernetes provisioning
• Container registry

Milestone Group 3

• PostgreSQL
• Redis
• Kafka or Redpanda
• Search
• Object storage

Milestone Group 4

• Kubernetes application deployment
• Helm charts
• API Gateway
• Backend services
• Workers
• Web application

Milestone Group 5

• CDN
• Ingress
• TLS
• Networking
• WebSocket infrastructure
• Media processing infrastructure

Milestone Group 6

• Secrets management
• Kubernetes security
• Container security
• Infrastructure security

Milestone Group 7

• GitHub Actions CI
• GitHub Actions CD
• Deployment validation
• Artifact promotion
• Rollback readiness

Milestone Group 8

• Prometheus
• Grafana
• Loki
• Tempo
• OpenTelemetry infrastructure
• Alerting
• SLOs

Milestone Group 9

• Backups
• Disaster recovery
• Runbooks
• Recovery testing

Milestone Group 10

• Load testing
• Security testing
• Performance validation
• Production hardening
• Infrastructure documentation

────────────────────────────────────────

PROJECT INDEX

Maintain a living Infrastructure Project Index.

After every milestone update:

• Current milestone
• Generated infrastructure files
• Docker components
• Docker Compose services
• Terraform modules
• Cloud resources
• Kubernetes resources
• Helm charts
• CI workflows
• CD workflows
• Monitoring components
• Alerting rules
• Backup components
• Disaster recovery procedures
• Runbooks
• Load-testing components
• Security controls
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

Every generated file must integrate with the completed application.

Do not regenerate unchanged files.

Only modify files when required.

────────────────────────────────────────

STOP CONDITIONS

Implement incrementally.

Each milestone should contain approximately 20–40 files.

At the end of every milestone:

1. Verify infrastructure consistency.
2. Verify application configuration compatibility.
3. Verify deployment dependencies.
4. Verify security configuration.
5. Verify observability integration.
6. Verify backup and recovery coverage.
7. Update the Infrastructure Project Index.
8. List completed infrastructure components.
9. Identify the exact next file or implementation unit.

STOP.

Wait for approval before generating the next milestone.

After the Infrastructure phase is complete, perform the final platform validation covering:

• Architecture consistency
• Backend integration
• Frontend integration
• Mobile integration
• Infrastructure integration
• Security
• Privacy
• Scalability
• Observability
• Disaster recovery
• Performance
• Testing
• Deployment readiness

The final result must be a production-ready enterprise social platform with reproducible infrastructure and a documented path to global scale.
