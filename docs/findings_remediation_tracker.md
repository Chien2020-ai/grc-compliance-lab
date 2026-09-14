# Findings and Remediation Tracker

This sample tracker demonstrates how findings move from identification through corrective action and closure verification.

| ID | Finding | Severity | Evidence | Owner | Corrective action | Target date | Status | Closure evidence |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| F01 | Quarterly access review did not include all privileged roles | High | Review export, IAM inventory | IT Operations | Update review population and repeat review for all privileged roles | 2026-10-15 | Open | Pending |
| F02 | One critical vulnerability is past the defined remediation window | High | Scan report, Jira ticket | Engineering | Apply remediation, retest, record exception if delayed | 2026-09-30 | In progress | Pending |
| F03 | Backup restoration has not been tested in the last 12 months | Medium | Backup schedule, recovery records | Platform Engineering | Perform restore test and document recovery result | 2026-10-31 | Open | Pending |
| F04 | Vendor retention terms are unclear for customer audio data | Medium | Vendor documentation, contract | Compliance Lead | Obtain written retention terms and confirm deletion options | 2026-10-10 | Open | Pending |
| F05 | Security incident contact list contains outdated personnel | Low | Incident response plan | Security Lead | Update contact list and confirm escalation ownership | 2026-09-20 | In progress | Pending |

## Closure criteria

A finding should not be closed only because the owner says the action is complete. Closure should be supported by evidence that the corrective action was implemented and that the original issue is no longer present.

For F01, acceptable closure evidence would include the updated access review population, the completed review, reviewer decisions, completed access changes, and confirmation that all privileged roles were included.

For F02, acceptable closure evidence would include the remediation ticket, deployment or configuration record, and a retest showing that the vulnerability is no longer detected.

## Root cause and corrective action example

### F01 Privileged access review population incomplete

**Immediate issue:** Several privileged roles were excluded from the quarterly review.

**Possible root cause:** The access review population was generated from a manually maintained list rather than the authoritative IAM source.

**Corrective action:** Generate future review populations from the authoritative IAM inventory and add a completeness check before each review starts.

**Effectiveness check:** Compare the next review population against the IAM inventory and confirm no privileged roles are missing.
