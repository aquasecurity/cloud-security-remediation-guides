[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Bucket Access Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Bucket Access Logging |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logging bucket has access logging enabled to detect tampering of log files |
| **More Info** | CloudTrail buckets should utilize access logging for an additional layer of auditing. If the log files are deleted or modified in any way, the additional access logs can help determine who made the changes. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/UG/ManagingBucketLogging.html |
| **Recommended Action** | Enable access logging on the CloudTrail bucket from the S3 console. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step2.png"/>
3. In the "Dashboard" panel click on the desired trail from the list under "Trails" to get to its configuration page.</br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step3.png"/>
4. Click on "Edit" under "General details".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step4.png"/>
5. Scroll down and under the "Storage location" option check the S3 bucket name which stores the log data.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step5.png"/>
6. Go to "Services" and search for "S3" to go into S3 buckets dashboard.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step6.png"/>
7. Select the "S3 bucket" which is used to store data log in CloudTrail and click on the bucket name to get to its configuration page.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step7.png"/>
8. Click the "Properties" tab from panel to get into Properties configuration options.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step8.png"/>
9. Scroll down to "Server Access Login" and check if its "Enabled" or not. If the "Server access logging" status shows "Disabled" then click "Edit" Button.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step9.png"/>
10. Select "Enable" and specify the "Target bucket" that will be used to store data log files.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step10.png"/>
11. Click on "Save changes" after review.</br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-access-logging/step11.png"/>
12. Repeat steps 3 to 11 for all other Cloudtrail Trails.
