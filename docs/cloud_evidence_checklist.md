# Cloud Evidence Checklist

This checklist uses a fictional AWS environment and focuses on the type of evidence that may support a control assessment.

| Control area | Example evidence request | What I would verify | Possible weakness |
| --- | --- | --- | --- |
| Identity and access | IAM user and role inventory, MFA configuration, access review records | Privileged access is limited, MFA is enforced, reviews are complete | Dormant or excessive privileges |
| Logging | CloudTrail configuration, log destination, retention settings | Relevant events are captured and retained | Logging disabled in a region or account |
| Encryption | S3, database, and volume encryption settings | Sensitive data is encrypted using approved methods | Unencrypted legacy resource |
| Network security | Security groups, VPC rules, public exposure inventory | Rules are justified and exposure is minimized | Broad inbound access |
| Secrets | Secrets Manager configuration, repository secret scanning | Secrets are not stored in source code and access is restricted | Hard coded credential or shared secret |
| Backup | Backup plans, success records, restore test evidence | Backups complete and recovery is tested | Backups exist but restoration has never been tested |
| Vulnerability management | Scan output, severity criteria, remediation tickets | Findings are assigned and closed within expected timelines | Critical issue past due |
| Change management | Pull request, approval, test evidence, deployment record | Changes are reviewed and traceable | Emergency or manual change with no approval record |
| Monitoring | Alert configuration, alert history, response record | Security relevant alerts are reviewed and acted on | Alert generated but no clear owner |
| Data retention | Storage lifecycle rules, retention schedule, deletion records | Technical settings match approved retention requirements | Policy and system configuration do not match |

## Example evidence review

### Access review

**Control objective:** Access remains appropriate to current responsibilities.

**Requested evidence:** Current IAM inventory, reviewer record, review decisions, completed access removals, and date of completion.

**Assessment questions:**

1. Does the population include all in scope users and privileged roles?
2. Was the reviewer independent enough to challenge inappropriate access?
3. Are exceptions documented?
4. Were removals actually implemented?
5. Is the evidence recent enough for the assessment period?

### Logging

**Control objective:** Security relevant activity can be reconstructed and investigated.

**Requested evidence:** CloudTrail settings, log storage configuration, retention period, sample events, and monitoring alerts.

A screenshot showing that CloudTrail is enabled would not by itself demonstrate that relevant logs are complete, protected, monitored, and retained for the required period.
