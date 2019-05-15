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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-logging/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-logging/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-logging/step4.png"/>
5. Click on the "Properties" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-logging/step5.png"/>
6. Check the "Server access logging" option under "Properties" and if it's set to "Disable logging" then S3 bucket logging is not enabled for the selected S3 bucket. </br><img src="/resources/aws/s3/s3-bucket-logging/step6.png"/>
7. Repeat steps number 2 - 6 to verify other S3 buckets in the region. </br>
8. Select the "S3 bucket" on which "Logging" needs to be enabled and click on the "Properties" tab. </br><img src="/resources/aws/s3/s3-bucket-logging/step8.png"/>
9. Click on the "Enable logging" option under "Server access logging" and choose the "Target bucket" from the dropdown menu for storing the logs and provide a unique name under "Target prefix" for the subdirectory where S3 logs will be stored. </br><img src="/resources/aws/s3/s3-bucket-logging/step9.png"/> 
10. Click on the "Save" button to make the necessary changes. </br><img src="/resources/aws/s3/s3-bucket-logging/step10.png"/>
11. Repeat steps number 8 - 10 to enable "Logging" for other S3 buckets.</br>
