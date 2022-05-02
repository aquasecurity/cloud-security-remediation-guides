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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br>![Step 2](/resources/aws/cloudtrail/cloudtrail-encryption/step2.png "Step 2 - Services")
3. In the "Dashboard" panel click on "View trails" button.</br> ![Step 3](/resources/aws/cloudtrail/cloudtrail-encryption/step3.png "Step 3 - Trails")
4. Select the "trail" that needs to be verified under "Name" column.</br>![Step 4](/resources/aws/cloudtrail/cloudtrail-encryption/step4.png "Step 4 - Name")
5. Scroll down and under the "Storage location" option check for "Encrypt log files with SSE-KMS". If its status is "No" the selected trail does not support log encryption.</br>![Step 5](/resources/aws/cloudtrail/cloudtrail-encryption/step5.png "Step 5 - SSE-KMS")
6. Click on the pencil icon to get into "Storage location" configuration settings. Scroll down and click on "Yes" next to "Encrypt log files with SSE-KMS" to enable the "CloudTrail" log encryption. </br> ![Step 6](/resources/aws/cloudtrail/cloudtrail-encryption/step6.png "Step 6 - Yes")
7. Click on the "Yes" option next to "Create a new KMS key" and enter a name. Make sure KMS key and S3 bucket must be in the same region.</br>![Step 7](/resources/aws/cloudtrail/cloudtrail-encryption/step7.png "Step 7 - Name")
8. Click on "No" option next to "Create a new KMS key" if already have "KMS key" available.</br>![Step 8](/resources/aws/cloudtrail/cloudtrail-encryption/step8.png "Step 7 - No")
9. Scroll down and click on "Save" to enable the CloudTrail log encryption.</br>![Step 9](/resources/aws/cloudtrail/cloudtrail-encryption/step9.png "Step 9 - Save")
