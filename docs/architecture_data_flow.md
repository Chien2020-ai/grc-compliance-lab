# Architecture and Data Flow

This document defines the fictional system boundary used throughout this portfolio lab.

## System overview

The example company provides a B2B SaaS application to customers in APAC. The application is hosted in AWS and integrates with several external SaaS providers.

### Main components

1. Web application used by customers and internal support staff
2. Application API hosted in AWS
3. PostgreSQL database containing account and application data
4. Object storage for documents and generated content
5. Central logging and monitoring
6. GitHub repository and CI/CD workflow
7. Identity provider for workforce access
8. External SaaS vendors for support, HR, analytics, and AI services

## Simplified data flow

Customer users submit account data and business content through the web application. The application sends requests to the API layer, which processes business logic and reads or writes data to the database and object storage.

Selected workflows may call approved third party services. Only the data required for the specific workflow should be shared with those vendors.

Application and infrastructure activity generates logs that are sent to the monitoring environment. Engineering changes are developed in GitHub, reviewed, tested, and deployed through the release process.

## Trust boundaries

### Customer boundary

Customer devices are outside the company controlled environment. Authentication, session management, transport encryption, and authorization are therefore important controls at the application boundary.

### Cloud boundary

AWS hosts the application, database, storage, logging, and supporting infrastructure. Cloud identity, configuration, encryption, network security, backup, and monitoring controls are in scope.

### Workforce boundary

Employees and contractors access company systems through managed identities. Access should be granted based on job responsibility and removed when no longer required.

### Third party boundary

External SaaS providers may process company or customer information. Their security posture, contractual commitments, data handling, subprocessors, and operational dependency should be assessed before and during use.

## Example data categories

| Data category | Example | Security concern |
| --- | --- | --- |
| Customer account data | Name, email, company, account ID | Privacy, unauthorized access |
| Authentication data | Account identifiers, tokens, session information | Account compromise |
| Business content | Customer submitted text, documents, audio | Confidentiality, vendor processing |
| Employee data | Workforce contact and HR information | Privacy, access restriction |
| Security logs | Authentication and system events | Integrity, retention, investigation |
| Configuration data | Cloud settings, secrets, deployment configuration | Privileged access, exposure |

## Compliance questions raised by the architecture

1. Which systems and data are included in the ISMS scope?
2. Where is sensitive data stored and processed?
3. Which third parties receive customer data?
4. What evidence demonstrates that access controls operate effectively?
5. How are logs protected and retained?
6. How are cloud changes reviewed and approved?
7. How are backups tested rather than only created?
8. How are customer deletion and retention requirements implemented technically?
9. Which responsibilities belong to the company and which belong to cloud or SaaS providers?
10. What evidence can be reused for ISO 27001, SOC 2, customer security reviews, and internal risk management?
