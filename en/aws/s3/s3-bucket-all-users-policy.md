[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket All Users Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket All Users Policy |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 bucket policies do not allow global write, delete, or read permissions |
| **More Info** | S3 buckets can be configured to allow the global principal to access the bucket via the bucket policy. This policy should be restricted only to known users or accounts. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/dev/using-iam-policies.html |
| **Recommended Action** | Remove wildcard principals from the bucket policy statements. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-all-users-policy/step4.png"/>
5. Click on the "Permissions" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-all-users-policy/step5.png"/>
6. Check the "Bucket Policy" option under "Properties" abd check the "Effect" and "Principal" value.If the "Effect" element value is set to "Allow" and the "Principal" element value is set to everyone ( * ) then the selected S3 bucket is publicly accessible. </br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step6.png"/>
7. Repeat steps number 2 - 6 to verify other S3 buckets in the region. </br>
8. Select the publicly accessible S3 bucket that needs to configure and click on the "Permissions" tab and click on the "Bucket Policy" option. </br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step8.png"/>
9. In the "Bucket Policy" option either remove the public accessibility by deleting the policy for the selected S3 bucket. Click on the "Delete" option at the top and click on "Delete" button on the "Delete Bucket Policy" tab.</br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step9.png"/>
10. In order to limit the public accessibility replace the Principal element current value with the Amazon Resource Name (ARN) ( e.g. { "AWS": "arn:aws:iam::102604298007:role/aws-elasticbeanstalk-ec2-role" } ) of the AWS account that should have access to the selected S3 bucket.</br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step10.png"/>
11. Click on the save button at the top to make the necessary changes. </br> <img src="/resources/aws/s3/s3-bucket-all-users-policy/step11.png"/>
12. Repeat steps number 8 - 11 to remove wildcard principals for other S3 buckets. </br>
