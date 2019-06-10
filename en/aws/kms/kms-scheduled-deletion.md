[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Scheduled Deletion

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Scheduled Deletion |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Detects KMS keys that are scheduled for deletion |
| **More Info** | Deleting a KMS key will permanently prevent all data encrypted using that key from being decrypted. Avoid deleting keys unless no encrypted data is in use. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/deleting-keys.html |
| **Recommended Action** | Disable the key deletion before the scheduled deletion time. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for KMS. </br> <img src="/resources/aws/kms/kms-scheduled-deletion/step2.png"/>
3. Scroll down the left navigation panel and choose "Customer Managed Keys" under "Key Management Service".</br> <img src="/resources/aws/kms/kms-scheduled-deletion/step3.png"/>
4. Verify the "KMS keys" that are scheduled for deletion and "Status" is shown as "Pending deletion" under the "Customer managed keys".</br> <img src="/resources/aws/kms/kms-scheduled-deletion/step4.png"/>
5. Repeat step number 2 - 4 to verify other "KMS keys" which are scheduled for deletion in other regions in AWS.</br>
6. Navigate to "Customer Managed Keys" under "Key Management Service" and select the "KMS key" that needs to modify to disable the scheduled key deletion.</br> <img src="/resources/aws/kms/kms-scheduled-deletion/step6.png"/>
7. Click on the "Key actions" button at the top and select the "Cancel key deletion" option to disable the scheduled deletion.</br> <img src="/resources/aws/kms/kms-scheduled-deletion/step7.png"/>
8. Click on the "Disable" option under "Key actions" to disable the selected "KMS key" instead of deleting the key.</br> <img src="/resources/aws/kms/kms-scheduled-deletion/step8.png"/>
9. Repeat steps number 6 - 8 to disable the key deletion before the scheduled deletion time.</br>
