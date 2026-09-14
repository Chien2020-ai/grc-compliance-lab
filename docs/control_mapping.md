# Control Mapping

This artifact shows how one security objective can support multiple frameworks. It is intentionally simplified for portfolio use and should not be treated as an official crosswalk.

| Security objective | ISO/IEC 27001:2022 reference | SOC 2 area | NIST aligned domain | Example evidence |
| --- | --- | --- | --- | --- |
| Restrict access based on business need | Annex A 5.15, 5.16, 5.18 | Logical access | Protect | Access matrix, role definitions, access review records |
| Protect privileged access | Annex A 8.2 | Logical access | Protect | Privileged account inventory, MFA settings, approval records |
| Record and monitor security events | Annex A 8.15, 8.16 | System operations | Detect | CloudTrail logs, SIEM alerts, retention settings, alert review records |
| Manage security incidents | Annex A 5.24 to 5.28 | System operations | Respond | Incident plan, ticket history, post incident review, lessons learned |
| Manage supplier security risk | Annex A 5.19 to 5.23 | Vendor management | Identify, Protect | Vendor inventory, due diligence, security questionnaire, contract clauses |
| Control software changes | Annex A 8.32 | Change management | Protect | Pull requests, approvals, test results, deployment records |
| Identify and remediate vulnerabilities | Annex A 8.8 | System operations | Identify, Protect | Scan reports, tickets, remediation SLA, retest evidence |
| Protect backups and recovery capability | Annex A 8.13, 5.30 | Availability | Recover | Backup configuration, restore test, recovery objectives, test report |
| Protect data throughout its lifecycle | Annex A 5.12, 5.14, 8.10, 8.24 | Confidentiality | Protect | Classification scheme, encryption settings, retention schedule, deletion evidence |
| Maintain audit ready evidence | Clauses 7.5, 9.1, 9.2, 10.1 | Monitoring and governance | Govern | Evidence index, internal audit records, corrective action tracker, review logs |

## How I would use this mapping

A control should not be implemented separately for every framework when the underlying objective is the same. I would first define the common control objective, identify the systems and owners involved, then map the evidence to each framework requirement.

For example, a quarterly access review can support several assurance needs if the review population is complete, the reviewer is appropriate, decisions are recorded, and removals are actually completed.

The goal is to reduce duplicate work while keeping the control traceable to each requirement.
