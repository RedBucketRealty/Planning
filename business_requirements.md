# Business Requirements for RedBucketRealty

## Sections

- [Business Requirements for RedBucketRealty](#business-requirements-for-redbucketrealty)
  - [Sections](#sections)
  - [Branding, Design, and Experiences](#branding-design-and-experiences)
  - [Messaging and Communication](#messaging-and-communication)
  - [Payments](#payments)
  - [Compliance](#compliance)
  - [Analytics](#analytics)
  - [Security and data](#security-and-data)
    - [User data](#user-data)
    - [Authentication, Authorization](#authentication-authorization)
  - [Product and Discovery](#product-and-discovery)
    - [Product types](#product-types)
    - [Product service](#product-service)
    - [Customer transactions](#customer-transactions)
    - [Customer fulfillment](#customer-fulfillment)
    - [Customer comfort](#customer-comfort)
  - [Social and sharing](#social-and-sharing)
  - [Referrals](#referrals)
  - [Service Level Objectives, and Indicators](#service-level-objectives-and-indicators)
    - [Scaling](#scaling)
    - [Confidentiality](#confidentiality)
    - [Integrity](#integrity)
    - [Availability](#availability)
    - [Reliability](#reliability)
    - [Resilience](#resilience)
    - [Cohesion and Coupling](#cohesion-and-coupling)
    - [Automation](#automation)
    - [Observability](#observability)
    - [Testing and Quality Assurance](#testing-and-quality-assurance)


## Branding, Design, and Experiences

- A set of color themes for light and dark modes.
  - Documentation for color themes.
- Design elements such as radii, spacing, sizing, etc should match brand aesthetics.
- A logo, multiple sizes.
- Design should have a clean aesthetic.
- Design should be accessible.
- A stylesheet should be developed.
- A collaboration cycle should be made.

## Messaging and Communication

- An asynchronous messaging service that allows customers to contact the business from within their accounts.
- A service that displays status of other services.
- An email service that automates transactional email for reminders and personalized messaging.
- A notifications service for sending automated notifications.

## Payments

- A payments service that integrates with a payments provider. It keeps track of the payment status.
- A service that displays current and next projected payments for the business.
- A service that tracks discount credits.

## Compliance

- A KYC intake service for individual and corporate users.
- A KYC verification service. It should delete data after it has been used, or within 30-90 days, whichever sooner.
- A service that allows business side modification of KYC data without disclosing stored data.
- A service that monitors internal compliance operations and audits.
- A service that securely signs and timestamps internal files.
- A service that securely signs and timestamps external files.
- A service for policy compliance automation, such as terms of use, agreements, contracts, etc.

## Analytics

- A fleet of services for analytics workloads.
- A fleet of ETL services for the following data:
  - Customer orders
  - Products
  - User trends
  - Referrals
  - Reviews
  - Surveys

## Security and data

- A data policy should be made.
- Data policy should follow all relevant laws, and be stored in accordance with industry best practices.
- Security decisions should be made in accordance with industry best practices, government recommendations, and recommendations from NIST (US).

### User data

- A service for user PII.
- User data should be stored according to data policy.
- User data should be exported to the user on request.
- User data should not have unrestricted access.

### Authentication, Authorization

- A service for handling IAM.
- A service for handling PAM.
- A service to test secrets against known breaches.

## Product and Discovery

### Product types

- These are the following types of products:
  1. Rent a residence (individual)
  2. Buy a residence (individual)
  3. Rent a private office (individual)
  4. Buy a private office (individual)
  5. Rent a shared co-working space (individual)
  6. Rent an event space (individual)
  7. Buy an event space (individual)
  8. Rent a warehouse (individual)
  9. Buy a warehouse (individual)
  10. Rent a virtual office space (individual)
  11. Rent a residence (corporate)
  12. Buy a residence (corporate)
  13. Rent a private office (corporate)
  14. Buy a private office (corporate)
  15. Rent a shared co-working space (corporate)
  16. Rent an event space (corporate)
  17. Buy an event space (corporate)
  18. Rent a warehouse (corporate)
  19. Buy a warehouse (corporate)
  20. Rent a virtual office space (corporate)

- These are the following services:
  1. Personalized real estate search
  2. Enterprise-wide realty provisioning
  3. Business office registration service

- These services are offered through partnerships and tie-ins:
  1. Food and catering
  2. Temporary workforce
  3. Office supplies
  4. Legal services
  5. General business services
  6. Event management
  7. Residential housekeeping
  8. Housekeeping services for enterprise needs
  9. General transportation and logistics
  10. Mail and package handling
  11. Warehouse management
  12. Real estate maintenance and renovation.

### Product service

- There should be a service for products data storage.
- There should be a service for product data ingestion.
- There should be a service for product data management.
- There should be a service for product procurement accessible by external partners.
- There should be a service for internal product compliance automation.
- A service to track installation and maintenance of products and services.

### Customer transactions

- A service for customer orders.
- A service for customer checkout process.
- A service to start checkout process from a QR code.
- A service to track future payments.
- A service to track usage, reviews, and help desk tickets related to 3rd party services.
- A service for 3rd party service partners to interface and communicate.

### Customer fulfillment

- A service for customer reviews and review management.
- A service for customer onboarding.
- A customer help desk service that communicates with the customer, resolves tickets, and tracks customer interactions.
- A live chat service for customers to connect to help desk service.

### Customer comfort

- A service for customer favorites.
- A service for customer wants. Public and anonymous displays of desire for a product.
- A service for deal notifications on selected services and products.
- A service to develop automated and custom deal campaigns on products and services.
- A service to develop automates and custom product recommendation campaigns on products and services.
- A service to develop automates and custom product highlighting campaigns on products and services
- A service for blog posts.
- A service for customer surveys.
- A service for customer brand loyalty rewards.
- A service for delivering insights to customers.
- There should be a service for product recommendations to customers.
- There should be a service for deal recommendations to customers.
- There should be a service for product highlighting across customer psychographics.

## Social and sharing

- A service for custom links to products optimized for social sharing.
- A service that creates custom links for customers to share and keep track of shared items.
- A service for communities based around users of a particular product.
- A service for internal communities, announcements, and discussions on products and services.

## Referrals

- A service for inbound customer referrals.
- A service for inbound partner referrals.

## Service Level Objectives, and Indicators

### Scaling

- Should scale to 10,000 users.

### Confidentiality

- Throughout the development and operations process, there should be a continuous maintenance of confidentiality of data, keys, connections, and service operations.

### Integrity

- Throughout the development and operations process, there should be a continuous maintenance of integrity of data, keys, connections, and service operations.

### Availability

- Throughout the development and operations process, data and service operations should be highly available.

### Reliability

- Throughout the development and operations process, service operations should be highly reliable.

### Resilience

- Throughout the development and operations process, service operations should be highly resilient.

### Cohesion and Coupling

- Throughout the development and operations process, data and service operations should be designed to have good cohesion and low or only necessary coupling.

### Automation

- Automation should be used throughout the development and operations processes.

### Observability

- Throughout the development and operations process, data and service operations should be designed to be observable.

### Testing and Quality Assurance

- Throughout the development and operations process, there should be automated testing and quality assurance procedures.
