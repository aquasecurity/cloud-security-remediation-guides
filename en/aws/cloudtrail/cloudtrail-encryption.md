[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Encryption |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail encryption at rest is enabled for logs |
| **More Info** | CloudTrail log files contain sensitive information about an account and should be encrypted at rest for additional protection. |
| **AWS Link** | http://docs.aws.amazon.com/awscloudtrail/latest/userguide/encrypting-cloudtrail-log-files-with-aws-kms.html |
| **Recommended Action** | Enable CloudTrail log encryption through the CloudTrail console or API |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step2.png"/>
3. In the "Dashboard" panel click on the desired trail from the list under "Trails" to get to its configuration page.</br> <img src="/resources/aws/cloudtrail/cloudtrail-encryption/step3.png"/>
4. Click on "Edit" button under "General details".</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step4.png"/>
5. On the Edit Trail page scroll down and check for "Log file SSE-KMS encryption". If its status is not selected as "Enabled" then the selected trail does not support log encryption.</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step5.png"/>
6. Select the checkbox to change the status as "Enabled under "Log file SSE-KMS encryption" to enable the "CloudTrail" log encryption. </br> <img src="/resources/aws/cloudtrail/cloudtrail-encryption/step6.png"/>
7. If you do not have an existing KMS key then under "Customer managed AWS KMS key" option select "New" and enter a name for "AWS KMS alias". Make sure KMS key and S3 bucket must be in the same region.</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step7.png"/>
8. If you already have "KMS key" available then under "Customer managed AWS KMS key" option select "Existing" and click to choose an existing key under "AWS KMS alias".
.</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step8.png"/>
9. Scroll down and click on "Save changes" to enable the CloudTrail log encryption.</br><img src="/resources/aws/cloudtrail/cloudtrail-encryption/step9.png"/>
