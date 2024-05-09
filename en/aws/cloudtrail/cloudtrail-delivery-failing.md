[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Delivery Failing

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Delivery Failing |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures that Amazon CloudTrail trail log files are delivered to destination S3 bucket. |
| **More Info** | Amazon CloudTrail trail logs should be delivered to destination S3 bucket to be used for security audits. |
| **AWS Link** | https://docs.aws.amazon.com/awscloudtrail/latest/userguide/how-cloudtrail-works.html |
| **Recommended Action** | Modify CloudTrail trail configurations so that logs are being delivered. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Navigate to Amazon [CloudTrail console](https://console.aws.amazon.com/cloudtrail/).
3. In the navigation panel, under CloudTrail, choose Trails.</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step3.png"/>
4. Click on the name of the Amazon CloudTrail trail that you want to modify.
5. In the General details section, choose Edit and perform the following steps:</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step5.png"/>
   a. Select Create new S3 bucket under Storage location to create the new target bucket.</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step5a.png"/>
   b. Provide a unique name for the new S3 bucket in the Trail log bucket and folder box.
   c. Choose Save changes to apply the changes. Once the target bucket is created, Amazon CloudTrail starts to deliver log files to the new S3 bucket and the Last log file delivered attribute value is updated.
6. Repeat steps no. 4 and 5 for each Amazon CloudTrail trail that you want to reconfigure in your AWS cloud account.