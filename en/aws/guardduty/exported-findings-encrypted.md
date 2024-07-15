# AWS / GuardDuty / Exported Findings Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Exported Findings Encrypted |
| **Cloud** | AWS |
| **Category** | GuardDuty |
| **Description** | Ensure that GuardDuty findings export is encrypted using desired KMS encryption level. |
| **More Info** | GuardDuty data, such as findings, is encrypted at rest using AWS owned customer master keys (CMK). Additionally, you can use your use key (CMKs) in order to gain more control over data encryption/decryption process. |
| **AWS Link** | https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_exportfindings.html |
| **Recommended Action** | Encrypt GuardDuty Export Findings with customer-manager keys (CMKs). |

## Detailed Remediation Steps