# GRC Compliance Lab

This repository is a hands on portfolio lab focused on technical GRC, security compliance, cloud evidence, vendor risk, and audit readiness.

It uses a fictional B2B SaaS company as the working scenario. The materials are created for learning and portfolio purposes. They do not represent a real client engagement, certification audit, or production compliance program.

## Scenario

The fictional company operates a cloud based SaaS platform used by business customers in APAC. It processes customer account data, employee information, application logs, and limited business content. The company is preparing for ISO/IEC 27001 and SOC 2 readiness while improving vendor risk management and customer security assurance.

The environment assumes AWS hosted workloads, GitHub based software delivery, SaaS vendors for business operations, role based access control, and a distributed team.

## What this lab demonstrates

1. Security risk assessment and risk register management
2. Control mapping across ISO/IEC 27001, SOC 2, and NIST aligned security domains
3. Evidence request design and evidence quality review
4. Cloud security and compliance evidence thinking
5. Vendor security assessment and residual risk decisions
6. Findings, remediation, ownership, and closure verification
7. Audit readiness and management reporting
8. Translating technical and regulatory requirements into operational actions

## Portfolio artifacts

| Artifact | Purpose |
| --- | --- |
| [Risk Register](docs/risk_register.md) | Shows risk identification, scoring, treatment, ownership, and residual risk thinking |
| [Control Mapping](docs/control_mapping.md) | Maps common security objectives across ISO/IEC 27001, SOC 2, and NIST aligned domains |
| [Cloud Evidence Checklist](docs/cloud_evidence_checklist.md) | Defines evidence that could support cloud control assessment |
| [Vendor Security Assessment](docs/vendor_security_assessment.md) | Demonstrates third party risk assessment from intake through residual risk |
| [Findings and Remediation Tracker](docs/findings_remediation_tracker.md) | Demonstrates issue ownership, corrective action, retest, and closure |
| [Architecture and Data Flow](docs/architecture_data_flow.md) | Documents the fictional system boundary and security relevant data flows |

## Working method

Each assessment follows the same reasoning pattern.

1. Define the business or security objective
2. Identify the relevant risk
3. Identify the expected control
4. Request evidence
5. Evaluate whether the evidence supports operating effectiveness
6. Record any gap or finding
7. Assign remediation ownership and due date
8. Verify closure with new evidence

## Evidence quality principles

Evidence is stronger when it is current, attributable, complete, reproducible, and directly connected to the control being assessed.

A policy alone does not prove that a control operates. For example, an access control policy may describe quarterly access reviews, but operating evidence would also be needed to show that reviews occurred, exceptions were handled, and changes were completed.

## APAC compliance lens

For an APAC deployment, security controls should also be reviewed against applicable privacy, contractual, and sector requirements. Areas requiring legal or privacy specialist validation may include Australian Privacy Principles, Singapore PDPA, cross border data transfer obligations, retention requirements, and customer specific regulated industry expectations.

This repository does not provide legal advice and does not claim professional implementation experience with those privacy regimes.

## About me

I am a product and project professional with experience across software, SaaS, data platforms, APIs, databases, cloud environments, and AI assisted workflows. I am building deeper hands on capability in technical GRC and security compliance. I completed an SGS delivered 40 hour ISO/IEC 27001:2022 Lead Auditor training course and the certification exam in September 2026, with certificate issuance pending.
