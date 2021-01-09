[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EFS / EFS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EFS Encryption Enabled |
| **Cloud** | AWS |
| **Category** | EFS |
| **Description** | Ensures that EFS volumes are encrypted at rest |
| **More Info** | EFS offers data at rest encryption using keys managed through AWS Key Management Service (KMS). |
| **AWS Link** | https://aws.amazon.com/blogs/aws/new-encryption-at-rest-for-amazon-elastic-file-system-efs/ |
| **Recommended Action** | Encryption of data at rest can only be enabled during file system creation. Encryption of data in transit is configured when mounting your file system. 1. Backup your data in not encrypted efs 2. Recreate the EFS and select 'Enable encryption of data at rest' |

## Detailed Remediation Steps




