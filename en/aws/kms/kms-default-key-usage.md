[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Default Key Usage

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Default Key Usage |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Checks AWS services to ensure the default KMS key is not being used |
| **More Info** | It is recommended not to use the default key to avoid encrypting disparate sets of data with the same key. Each application should have its own customer-managed KMS key |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/concepts.html |
| **Recommended Action** | Avoid using the default KMS key |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for KMS. </br> <img src="/resources/aws/kms/kms-default-key-usage/step2.png"/>
3. Scroll down the left navigation panel and choose "AWS managed keys" under "Key Management Service".</br> <img src="/resources/aws/kms/kms-default-key-usage/step3.png"/>
4. Select the "KMS key" that needs to be verified by clicking on the alias of the key under "Alias".</br> <img src="/resources/aws/kms/kms-default-key-usage/step4.png"/>
5. On the "AWS managed keys" page verify the "General configuration" and check the "Description" tab. If "Default master key"(for e.g. aws/ebs) is showing than the selected "Amazon KMS key" is a default master key.</br> <img src="/resources/aws/kms/kms-default-key-usage/step5.png"/>
6. Naviagte to the "EC2 dashboard" and select the "Snapshots" under "ELASTIC BLOCK STORE".</br> <img src="/resources/aws/kms/kms-default-key-usage/step6.png"/>
7. Select the "Snapshot" that needs to be verified and check the "Description" tab from the bottom panel. Check the "KMS Key Aliases" and if the value is set to "aws/ebs then the selected EBS volume is using the default master key.</br> <img src="/resources/aws/kms/kms-default-key-usage/step7.png"/>
8. Repeat steps number 2 - 7 to verify other "KMS Default keys Usage" in the selected region.</br>
9. Navigate to "KMS key" dashbaord and click on the "Create key" button at the top panel to create a new "KMS key".</br> <img src="/resources/aws/kms/kms-default-key-usage/step9.png"/>
10. On the "Add alias and description" page provide the "Alias" and "Description" for the new "KMS key" and click on the "Next" button. </br> <img src="/resources/aws/kms/kms-default-key-usage/step10.png"/>
11. On the "Add tags" page provide a unique key for "Tag key","Tag value" and click on the "Next" button.</br> <img src="/resources/aws/kms/kms-default-key-usage/step11.png"/>
12. On the "Define key administrative permissions" page select the "IAM users" and roles who can administer the new "KMS key" through the KMS API.</br> <img src="/resources/aws/kms/kms-default-key-usage/step12.png"/>
13. Click on the "Next" button at the bottom to continue the new "KMS key" process.</br> <img src="/resources/aws/kms/kms-default-key-usage/step13.png"/>
14. On the "Define key usage permissions" page select the IAM users and roles that can use the CMK to encrypt and decrypt data with the "AWS KMS API" and click on the "Next" button.<br> <img src="/resources/aws/kms/kms-default-key-usage/step14.png"/>
15. On the "Review and edit key policy" page review the policy and click on the "Finish" button to create a new "KMS key" which can be used to encrypt/decrypt the data.</br> <img src="/resources/aws/kms/kms-default-key-usage/step15.png"/>
16. Replace the "Default KMS key" with newly created "Customer managed key".</br>
17. Repeat steps number 9 - 16 to avoid using the default KMS key.</br>
