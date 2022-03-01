[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Logging |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 bucket logging is enabled for S3 buckets |
| **More Info** | S3 bucket logging helps maintain an audit trail of                 access that can be used in the event of a security                 incident. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/Logging.html |
| **Recommended Action** | Enable bucket logging for each S3 bucket. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-logging/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-logging/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-logging/step4.png"/>
5. Click on the "Properties" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-logging/step5.png"/>
6. Check the "Server access logging" option under "Properties" and if it's set to "Disabled" then S3 bucket logging is not enabled for the selected S3 bucket. </br><img src="/resources/aws/s3/s3-bucket-logging/step6.png"/>
7. To enable Server access logging click on the "Edit " button  under "Server access logging" option. On the "Edit server access logging" page select "Enable" and choose the "Target bucket" from the dropdown menu for storing the logs.</br><img src="/resources/aws/s3/s3-bucket-logging/step7.png"/>
8. Click on the "Save changes" button to make the necessary changes. </br><img src="/resources/aws/s3/s3-bucket-logging/step8.png"/>
9. Repeat steps number 8 - 10 to enable "Logging" for other S3 buckets.</br>
