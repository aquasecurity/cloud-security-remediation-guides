[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Glacier / S3 Glacier Vault Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Glacier Vault Public Access |
| **Cloud** | AWS |
| **Category** | Glacier |
| **Description** | Ensure that S3 Glacier Vault public access block is enabled for the account |
| **More Info** | Blocking S3 Glacier Vault public access at the account level ensures objects are not accidentally exposed |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html |
| **Recommended Action** | Add access policy for the S3 Glacier Vault to block public access for the AWS account |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for S3 Glacier. </br> <img src="/resources/aws/glacier/s3-glacier-vault-public-access/step2.png" />
3. On the navigation pane to the left, click on vaults. </br><img src="/resources/aws/glacier/s3-glacier-vault-public-access/step3.png" />
4. Click the vault name that you need you need to edit its policy to block public access. </br><img src="/resources/aws/glacier/s3-glacier-vault-public-access/step4.png" />
5. Select Vault Policies tab. </br><img src="/resources/aws/glacier/s3-glacier-vault-public-access/step5.png" />
6. Click on Edit vault access policy. </br><img src="/resources/aws/glacier/s3-glacier-vault-public-access/step6.png" />
7. Edit the policy by removing public access (e.g. "Resource": "*" or "Principal": "*", and "Effect": "Allow") and make sure the policy grant access only to fixed values (values that don't contain a wildcard or an AWS Identity and Access Management Policy Variable). </br>
8. See this resource to understand when a policy considered public: https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-block-public-access.html#access-control-block-public-access-policy-status </br>