# Vendor Security Assessment

This sample demonstrates a basic third party risk workflow using a fictional AI SaaS vendor.

## Vendor profile

**Vendor:** VoiceFlow AI Services, fictional

**Service:** Hosted AI voice and transcription API

**Business use:** Customer support workflow

**Data involved:** Customer contact details, audio content, support metadata

**Criticality:** High

**Integration type:** API

## Inherent risk considerations

| Area | Question | Initial assessment |
| --- | --- | --- |
| Data sensitivity | Does the vendor process confidential or personal data? | Yes |
| Privileged access | Does the vendor have access to production systems? | Limited through API integration |
| Availability | Would an outage affect a customer facing process? | Yes |
| Subprocessors | Does the service rely on additional third parties? | Requires review |
| Cross border processing | Could data be stored or processed outside the primary customer region? | Requires confirmation |
| AI specific use | Is customer content processed by an AI model? | Yes |
| Regulatory impact | Could regulated customers require additional controls or contractual commitments? | Yes |

## Evidence request

1. Current ISO 27001 certificate or equivalent independent assurance evidence
2. SOC 2 report if available
3. Data processing terms and subprocessor list
4. Data retention and deletion documentation
5. Encryption practices for data in transit and at rest
6. Access control and privileged access practices
7. Incident notification commitments
8. Business continuity and disaster recovery summary
9. Vulnerability management process
10. AI data usage and model training policy

## Example challenge questions

**Retention:** If the vendor states that customer content is deleted after a defined period, how is deletion enforced and can enterprise customers configure a shorter period?

**AI data use:** Is customer input used for model training, quality improvement, or human review? What controls and customer choices apply?

**Subprocessors:** Which subprocessors can receive customer content and in which regions is the data processed?

**Access:** Under what circumstances can vendor personnel access customer content, and how is that access approved, logged, and reviewed?

**Incidents:** What contractual notification timeline applies when an incident affects customer data?

## Example assessment outcome

**Inherent risk:** High

**Key gap:** Data retention and regional processing commitments require clarification before use with regulated customer data.

**Proposed treatment:** Limit initial use to lower sensitivity workflows until contractual and technical requirements are confirmed. Require security and legal review before expanding scope.

**Residual risk:** Medium, assuming the required commitments and controls are validated.

## Ongoing monitoring

A completed vendor assessment should not be considered permanent. Reassessment may be triggered by major service changes, new subprocessors, security incidents, material contract changes, new data types, or the normal review cycle.
