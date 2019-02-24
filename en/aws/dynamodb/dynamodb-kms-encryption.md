[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / DynamoDB / DynamoDB KMS Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | DynamoDB KMS Encryption |
| **Cloud** | AWS |
| **Category** | DynamoDB |
| **Description** | Ensures DynamoDB tables are encrypted using a customer-owned KMS key. |
| **More Info** | DynamoDB tables can be encrypted using AWS-owned or customer-owned KMS keys. Customer keys should be used to ensure control over the encryption seed data. |
| **AWS Link** | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/EncryptionAtRest.html |
| **Recommended Action** | Create a new DynamoDB table using a CMK KMS key. |

## Detailed Remediation Steps

