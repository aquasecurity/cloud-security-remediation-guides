[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Encryption Enabled |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EBS volumes are encrypted at rest |
| **More Info** | EBS volumes should have at-rest encryption enabled through AWS using KMS. If the volume is used for a root volume, the instance must be launched from an AMI that has been encrypted as well. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html |
| **Recommended Action** | Enable encryption for EBS volumes. |

## Detailed Remediation Steps

