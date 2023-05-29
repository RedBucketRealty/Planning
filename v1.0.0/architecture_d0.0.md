# Architecture: v1.0.0

## Sections

- [Architecture: v1.0.0](#architecture-v100)
  - [Sections](#sections)
  - [IAM](#iam)
  - [PAM](#pam)
  - [Pwned Passwords service](#pwned-passwords-service)
  - [User data service](#user-data-service)
  - [Email service](#email-service)
  - [Policy Compliance automation service](#policy-compliance-automation-service)
  - [Product service](#product-service)
  - [Orders service](#orders-service)
  - [Payments service](#payments-service)
  - [Onboarding service](#onboarding-service)
  - [KYC services](#kyc-services)
    - [KYC storage service](#kyc-storage-service)
    - [KYC verification service](#kyc-verification-service)
  - [File signing service](#file-signing-service)

## IAM

- IAM authorization and authentication should be time limited.
- IAM should allow ABAC, RBAC.
- It should be possible to quickly authenticate requests to services using tokens.
- IAM service should notify users when an event related to their authentication and authorization happens.
- IAM should employ multi-factor authentication whenever possible.
- IAM should offer a versioned and robust programmable interface for automation.
- IAM service should be idempotent.
- IAM should offer a UI console for manual engineering.
- An off the shelf and cloud agnostic IAM service should be developed.
- IAM service should be scalable, containerized, and cloud native.
- IAM service should be designed to fail and degrade gracefully.
- IAM service should offer simple and reliable interfaces for IT administration without requiring significant technical knowledge about the service.
- Supports detailed, auditable, timestamped logs for all operations.
- IAM should alert on unusual access patterns.
- IAM service should employ it's own separate storage solutions.
- IAM data should be encrypted at rest, and while in transit.
- IAM service should use soft deletion techniques.
- IAM service should have pagination and sorting built in, with the results restricted to one (1) for now.
- IAM service should be designed with pluralization and multi-tenancy, including structure and architecture, in mind.
- IAM backup, migration, and restore should be tested and automated.
- IAM data transmission should be minimized and compressed for efficiency.
- IAM should be structured to reduce blast radius in general, and between company and user data in case of compromise, using segmentation at the service data level.
- IAM should be developed while using static and dynamic security and quality control tools during the development and operations process.
- Authentication tokens should be versioned, and include suffix and prefixes.
- IAM service should define an error budget.
- IAM service deployment and cleanup should be automated.
- IAM service deprecation and sunset should be planned and designed for.
- IAM service should be designed with observability and ease of debugging in mind.
- IAM service should have latency and speed benchmark targets.
- IAM service should allow export of certain data, in compliance with laws and regulations.

## PAM

- PAM should be used to store secrets for cloud native environments.
- PAM should allow automatic and periodical secret rollover.
- Access to PAM admin should be limited to minimize exposure.
- Should integrate with IAM service.

- PAM should employ multi-factor authentication whenever possible.
- PAM should offer a versioned and robust programmable interface for automation.
- PAM service should be idempotent.
- PAM should offer a UI console for manual administration.
- An off the shelf and cloud agnostic PAM service should be developed.
- PAM service should be scalable, containerized, and cloud native.
- PAM service should be designed to fail and degrade gracefully.
- PAM service should offer simple and reliable interfaces for IT administration without requiring significant technical knowledge about the service.
- Supports detailed, auditable, timestamped logs for all operations.
- PAM should alert on unusual access patterns.
- PAM service should employ it's own separate storage solutions.
- PAM data should be encrypted at rest, and while in transit.
- PAM service should use soft deletion techniques.
- PAM service should have pagination and sorting built in, with the results restricted to one (1) for now.
- PAM service should be designed with pluralization and multi-tenancy, including structure and architecture, in mind.
- PAM backup, migration, and restore should be tested and automated.
- PAM data transmission should be minimized and compressed for efficiency.
- PAM should be structured to reduce blast radius in case of compromise, using segmentation at the service data level.
- PAM should be developed while using static and dynamic security and quality control tools during the development and operations process.
- Generated PAM tokens should be versioned, and include suffix and prefixes.
- PAM service should define an error budget.
- PAM service deployment and cleanup should be automated.
- PAM service deprecation and sunset should be planned for.
- PAM service should be designed with observability and ease of debugging in mind.
- PAM service should have latency and speed benchmark targets.
- PAM service should allow export of certain data, in compliance with laws and regulations.

## Pwned Passwords service

A service to check passwords against known breaches.

- Compares password hashes against known breaches.
- Integrates with IAM service.
- Can be called by internal services and external entities.

## User data service

A service for customer user data.

- Has multiple authorization levels for all operations.
- Supports detailed, auditable logs for all operations.
- Stores data in user database.
- Allows users to request archive of user data.
- Data should be encrypted during transport.
- Data should be encrypted during rest.
- Supports CRUD operations on user database.
- Data access should be restricted according to data policy.
- Automates removal of data according to data policy.
- Automates archiving of data according to data policy.

## Email service

An email service that automates transactional email for reminders and personalized messaging.

- Integrates with IAM service.
- Integrates with user data service.
- Allows access to only internal services.
- Allows sending emails to pre-specified recipient addresses.
- Allows configuration of fine grained limits on addition of recipient addresses.
- Archives email data.
- Supports detailed, auditable logs for all operations.
- Allows configuration of fine grained transaction limits.
- Allows configuration of templates for personalized messaging.
- Allows configuration of scheduled transactions for automated reminders.

## Policy Compliance automation service

A service for policy compliance automation, such as terms of use, agreements, contracts, etc.

- Integrates with IAM service.
- Integrates with user data service.
- Integrates with file signing service.
- Integrates with email service.
- Has multiple authorization levels for all operations.
- Supports detailed, auditable logs for all operations.
- Allows multiple users to automatically sign and timestamp policy agreements and automate other compliance needs.
- Allows creation of policy templates.
- Allows asking for explicit authorization and consent before automating compliance.
- Archives policy and compliance data.

## Product service

A service for storing product data. Allows read operations on the product database.

- Has multiple authorization levels for read access.

A service that should bulk ingest product data into the product database. Acts with a read-only-once message queue.

- It should allow upload only to authorized internal users.

A service for product data management.

- Allows access to only authorized internal users.
- Has multiple authorization levels for all operations.
- Integrates with product compliance automation service.
- Integrates with bulk ingest product data service.
- Allows CRUD operations on the product database.
- Allows changing of data access authorization levels of the product data by authorized users.

A service for internal product compliance management.

- Allows management of compliance requirements across product classes.
- Allows access only to authorized internal users.
- Automates part of compliance workflow for products and services.
- Allows compliance specialists to execute appropriate compliance actions.
- Generate auditable logs for each compliance requirement and action.

A service to evaluate and manage products and product categories.

- Integrates with analytics services to display analytics insights.
- Allows access to only authorized internal users.
- Allows taking products and services on and off the shelf.
- Allows application of discounts and promotional campaigns.

## Orders service

A service for customer orders.

- Integrates with the payment service.
- Integrates with the messaging service.
- Integrates with the analytics service.
- Integrates with the policy compliance automation service.
- Allows CRU operations on orders database.
- Has multiple authorization levels for all operations.
- Allows filter and sort queries for orders.
- Allows bulk download of order data.
- Allows internal users to create, read, or update orders.
- Stores relevant legal, KYC, and order data with each order.
- Allows CRU operations on invoices.
- Generates invoices in multiple formats.
- Stores invoice data in orders database.
- Stores invoice files in object storage.
- Allows bulk download of invoice data and files.
- Sends order status updates.
- Unpaid orders are cancelled after a configured amount of time.

## Payments service

A payments service that integrates with a payments provider. It keeps track of the payment status.

- Has multiple authorization levels for all operations.
- Integrates with the orders service.
- Integrates with external payments providers.
- Integrates with policy compliance automation service.
- Stores items in a cart for checkout.
- Ensures necessary KYC steps have been completed before processing.
- Ensures all policy compliance steps have been completed before processing.
- Stores only relevant payments data.

A service that archives all data associated with every payment for compliance assurance.

- Integrates with the orders service.
- Integrates with the user data service.
- Integrates with email service.
- Integrates with the policy compliance automation service.
- Stores all relevant data together in object database.
- Supports detailed, auditable logs for all operations.

## Onboarding service

A service for customer onboarding after signup. All consumer users must perform onboarding, and access should be restricted depending on the level of onboarding completed.

- Integrates with user data service.
- Integrates with KYC service.

## KYC services

### KYC storage service

A service for secure KYC information transfer.

- Integrates with user data service.
- Integrates with KYC verification service.
- Stores data in KYC database.
- Data should be encrypted during transport.
- Data should be encrypted during rest.
- Supports CRUD operations on KYC database.
- Data access should be restricted as much as possible.
- Has multiple authorization levels for all operations.
- Supports detailed, auditable logs for all operations.

### KYC verification service

A service for verification of KYC data through automation and by authorized personnel.

- Integrates with user data service.
- Integrates with KYC storage service.
- Integrates with external services for KYC verification automation.
- Provides an interface for authorized personnel to perform manual verification tasks.
- Automates removal of user KYC data according to policy.
- Data access should be restricted as much as possible.
- Has multiple authorization levels for all operations.
- Supports detailed, auditable logs for all operations.
- Allows access to only authorized internal users.

## File signing service

A service that securely signs and timestamps internal files.

- Has multiple authorization levels for all operations.
- Allows access only to authorized internal users.
- Supports detailed, auditable logs for all operations.
- Allows automated signing of files by internal services.
- Allows internal users to sign files.
- Generates and stores timestamps using a timestamp server.
- Supports verification and display of signature status of files.
- Allows multiple users to sign multiple files in one operation.
