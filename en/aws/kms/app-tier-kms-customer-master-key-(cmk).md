[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / App-Tier KMS Customer Master Key (CMK)

## Quick Info

| | |
|-|-|
| **Plugin Title** | App-Tier KMS Customer Master Key (CMK) |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Ensures that there is one Amazon KMS Customer Master Key (CMK) present in the account for App-Tier resources. |
| **More Info** | Amazon KMS should have Customer Master Key (CMK) for App-Tier to protect data in transit. |
| **AWS Link** | https://docs.aws.amazon.com/kms/latest/developerguide/create-keys.html |
| **Recommended Action** | Create a Customer Master Key (CMK) with App-Tier tag |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for KMS. </br>
3. To change the AWS Region, use the Region selector in the upper-right corner of the page. </br>
4. In the navigation pane, choose Customer managed keys. </br>
5. Choose Create key. </br>
4. Select the key type. If you are creating a KMS key to encrypt data you store or manage in an AWS service, create a symmetric encryption KMS key, this list of AWS services that are integrated with AWS KMS use only symmetric encryption KMS keys https://aws.amazon.com/kms/features/#AWS_Service_Integration. </br>
5. For help deciding which type of KMS key to create see https://docs.aws.amazon.com/kms/latest/developerguide/key-types.html#symm-asymm-choose </br>
6. On the "Add alias and description" page provide the "Alias" and "Description" for the new "KMS key" and click on the "Next" button. </br> 
7. On the "Add tags" page provide a unique key for "Tag key","Tag value" and click on the "Next" button.</br>
8. On the "Define key administrative permissions" page select the "IAM users" and roles who can administer the new "KMS key" through the KMS API.</br> 
9. Click on the "Next" button at the bottom to continue the new "KMS key" process.</br> 
10. On the "Define key usage permissions" page select the IAM users and roles that can use the CMK to encrypt and decrypt data with the "AWS KMS API" and click on the "Next" button.<br> 
11. On the "Review and edit key policy" page review the policy and click on the "Finish" button to create a new "KMS key" which can be used to encrypt/decrypt the data.</br>