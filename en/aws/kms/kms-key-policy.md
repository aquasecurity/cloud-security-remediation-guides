[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Key Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Key Policy |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Validates the KMS key policy to ensure least-privilege access. |
| **More Info** | KMS key policies should be designed to limit the number of users who can perform encrypt and decrypt operations. Each application should use its own key to avoid over exposure. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html |
| **Recommended Action** | Modify the KMS key policy to remove any wildcards and limit the number of users and roles that can perform encrypt and decrypt operations using the key. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for KMS. </br> <img src="/resources/aws/kms/kms-key-policy/step2.png"/>
3. Scroll down the left navigation panel and choose "Customer managed keys" under "Key Management Service".</br> <img src="/resources/aws/kms/kms-key-policy/step3.png"/>
4. Select the "KMS key" that needs to be verified.</br> <img src="/resources/aws/kms/kms-key-policy/step4.png"/>
5. On the "Customer managed keys" page scroll down and on the "Key policy" tab click on the "Switch to policy view" button.</br> <img src="/resources/aws/kms/kms-key-policy/step5.png"/>
6. In the "key policy" tab if the "Principal" element value is set to ("AWS" : * ) and there are no Condition clauses to filter the access then the selected "KMS policy" is using wildcards.</br> <img src="/resources/aws/kms/kms-key-policy/step6.png"/>
7. Repeat step number 2 - 6 to verify other "KMS key" in the region.</br>
8. Navigate to "Customer Managed Keys" under "Key Management Service" and select the "KMS key" that needs to modify to restrict the he number of users and roles that can perform encrypt and decrypt operation and have any wildcards.</br> <img src="/resources/aws/kms/kms-key-policy/step8.png"/>
9. On the "Customer managed keys" page scroll down and on the "Key policy" tab click on the "Switch to policy view" button and replace the "Everyone" grantee ("AWS" : * )  from the Principal element value with an "AWS account ID" or "AWS ARN" and click on the "Save" changes button.</br> <img src="/resources/aws/kms/kms-key-policy/step9.png"/>
10. Restrict the number of users and roles that can use the selected "KMS key" for encrypt and decrypt operations by making each application should use its own key .</br> 
11. Repeat steps number 7 - 10 to modify the "KMS key" policy of other "KMS keys" in the selected region.</br>
