[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Versioning

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Versioning |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures object versioning is enabled on S3 buckets |
| **More Info** | Object versioning can help protect against the overwriting of                 objects or data loss in the event of a compromise. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html |
| **Recommended Action** | Enable object versioning for buckets with                         sensitive contents at a minimum and for all buckets                         ideally. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-versioning/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-versioning/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-versioning/step4.png"/>
5. Click on the "Properties" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-versioning/step5.png"/>
6. Check the "Versioning" option under "Properties" and if it's set to "Suspend versioning" then S3 bucket versioning is not enabled for the selected S3 bucket. </br><img src="/resources/aws/s3/s3-bucket-versioning/step6.png"/>
7. Repeat steps number 2 - 6 to verify other S3 buckets in the region. </br>
8. Select the "S3 bucket" on which versioning needs to be enabled and click on the "Properties" tab. </br><img src="/resources/aws/s3/s3-bucket-versioning/step8.png"/>
9. Click on the "Enable versioning" option under "Versioning".</br><img src="/resources/aws/s3/s3-bucket-versioning/step9.png"/>
10. Click on the "Save" button to make the necessary changes. </br><img src="/resources/aws/s3/s3-bucket-versioning/step10.png"/>
11. Repeat steps number 8 - 10 to enable versioning for other S3 buckets.</br>

