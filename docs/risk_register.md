# Risk Register

This sample risk register is part of the fictional SaaS scenario described in the main README.

## Scoring method

Likelihood and impact are scored from 1 to 5. Inherent risk is calculated before considering controls. Residual risk reflects the expected level after treatment.

| ID | Risk scenario | Asset or process | Likelihood | Impact | Inherent risk | Existing or planned controls | Treatment | Owner | Residual risk |
| --- | --- | --- | ---: | ---: | ---: | --- | --- | --- | ---: |
| R01 | Compromised privileged account leads to unauthorized access to production data | AWS production environment | 3 | 5 | 15 | MFA, role based access, privileged access review, logging | Reduce | Security Lead | 6 |
| R02 | Excessive user permissions remain after role changes | Identity and access management | 4 | 4 | 16 | Joiner mover leaver process, quarterly access review | Reduce | IT Operations | 8 |
| R03 | Security logs are incomplete or unavailable during an incident | Logging and monitoring | 3 | 5 | 15 | Centralized logging, retention settings, alerting | Reduce | Platform Engineering | 6 |
| R04 | Sensitive data is exposed through misconfigured cloud storage | Customer data | 3 | 5 | 15 | Encryption, access restrictions, configuration review | Reduce | Platform Engineering | 5 |
| R05 | Critical SaaS vendor suffers an outage or security incident | Third party services | 4 | 4 | 16 | Vendor assessment, contractual requirements, backup procedures | Reduce | Operations | 8 |
| R06 | Software change introduces a security weakness into production | SDLC | 3 | 4 | 12 | Code review, change approval, testing, dependency scanning | Reduce | Engineering | 6 |
| R07 | Backups exist but cannot be restored within business requirements | Business continuity | 3 | 5 | 15 | Scheduled backups, restore testing, documented recovery objectives | Reduce | Platform Engineering | 6 |
| R08 | Departing employee retains access to company systems | Offboarding | 3 | 4 | 12 | HR notification, account disablement checklist, access verification | Reduce | IT Operations | 4 |
| R09 | Customer security commitments are accepted without confirming control capability | Sales and customer assurance | 3 | 4 | 12 | Security review of questionnaires and contractual commitments | Reduce | Compliance Lead | 6 |
| R10 | API secrets are exposed in code or shared insecurely | Application development | 3 | 5 | 15 | Secret management, repository scanning, access restrictions | Reduce | Engineering | 5 |
| R11 | Vendor access to sensitive systems is broader than required | Third party access | 3 | 4 | 12 | Least privilege, time limited access, vendor access review | Reduce | IT Operations | 5 |
| R12 | Retention settings conflict with customer or privacy requirements | Data lifecycle | 3 | 4 | 12 | Retention schedule, system configuration review, legal validation | Reduce | Compliance Lead | 6 |
| R13 | Incident response roles are unclear during a high severity event | Incident management | 3 | 5 | 15 | Incident response plan, escalation matrix, tabletop exercise | Reduce | Security Lead | 6 |
| R14 | Vulnerabilities remain open beyond the accepted remediation window | Vulnerability management | 4 | 4 | 16 | Severity based SLA, ticket ownership, retest and closure | Reduce | Engineering | 8 |
| R15 | Compliance evidence becomes stale and no longer reflects actual control operation | Audit readiness | 4 | 3 | 12 | Evidence owners, review cadence, evidence repository, expiry tracking | Reduce | Compliance Lead | 6 |

## Example risk treatment notes

### R02 Excessive permissions

The control objective is to ensure access remains appropriate to current job responsibilities. Evidence should include the access review population, reviewer identity, decisions, exceptions, completed removals, and completion date.

### R05 Third party service disruption

Vendor assurance should consider both security and operational dependency. A strong assessment would review service criticality, data access, incident notification terms, continuity commitments, available assurance reports, and contingency options.

### R15 Stale compliance evidence

Evidence collection should not be treated as a one time exercise. Each artifact should have an owner, source, review date, expected refresh frequency, and clear connection to the control being assessed.
