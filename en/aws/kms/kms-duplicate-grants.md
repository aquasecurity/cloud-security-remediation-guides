[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Duplicate Grants

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Duplicate Grants |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Ensure that AWS KMS keys does not have duplicate grants to adhere to AWS security best practices. |
| **More Info** | Duplicate grants have the same key ARN, API actions, grantee principal, encryption context, and name. If you retire or revoke the original grant but leave the duplicates, the leftover duplicate grants constitute unintended escalations of privilege. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/concepts.html |
| **Recommended Action** | Delete duplicate grants for AWS KMS keys |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for KMS. </br>
3. To delete a grant, retire it or revoke it. </br>
4. To identify the grant to retire, use a grant token, or both the grant ID and a key identifier (key ID or key ARN) of the KMS key. </br>
5. Follow this guide https://docs.aws.amazon.com/kms/latest/APIReference/API_RetireGrant.html to retire grant either by sending a request or using language-specific AWS SDKs. </br> 
6. To revoke a grant follow this document https://docs.aws.amazon.com/kms/latest/APIReference/API_RevokeGrant.html </br>