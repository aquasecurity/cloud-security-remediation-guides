[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Encrypted Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Encrypted Snapshots |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EBS snapshots are encrypted at rest |
| **More Info** | EBS snapshots should have at-rest encryption enabled through AWS using KMS. If the volume was not encrypted and a snapshot was taken the snapshot will be unencrypted. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html#encryption-support |
| **Recommended Action** | Configure volume encryption and delete unencrypted EBS snapshots. |

## Detailed Remediation Steps

