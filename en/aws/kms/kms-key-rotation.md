[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Key Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Key Rotation |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Ensures KMS keys are set to rotate on a regular schedule |
| **More Info** | All KMS keys should have key rotation enabled. AWS will handle the rotation of the encryption key itself, as well as storage of previous keys, so previous data does not need to be re-encrypted before the rotation occurs. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html |
| **Recommended Action** | Enable yearly rotation for the KMS key |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for KMS. </br> <img src="/resources/aws/kms/kms-key-rotation/step2.png"/>
3. Scroll down the left navigation panel and choose "Customer Managed Keys" under "Key Management Service".</br> <img src="/resources/aws/kms/kms-key-rotation/step3.png"/>
4. Select the key that needs to be verified by clicking on the alias of the key under "Alias".</br> <img src="/resources/aws/kms/kms-key-rotation/step4.png"/>
5. Scroll down the "Customer managed keys" page and click on the "Key rotation" and check the "Automatically rotate this CMK every year" status. If it's not checked then the selected "KMS key" is not set to rotate on a regular schedule.</br> <img src="/resources/aws/kms/kms-key-rotation/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "KMS keys" in the selected AWS region.</br>
7. Navigate to "Customer Managed Keys" under "Key Management Service" and select the "KMS key" that needs to modify to enable yearly rotation for the KMS key.</br> <img src="/resources/aws/kms/kms-key-rotation/step7.png"/>
8. Scroll down the "Customer managed keys" page and click on the "Key rotation" tab. Enable "Automatically rotate this CMK every year" checkbox and click on the "Save" button to make the necessary changes.</br> <img src="/resources/aws/kms/kms-key-rotation/step8.png"/>
9. Repeat steps number 7 - 8 to enable yearly rotation for the "KMS key".</br>
