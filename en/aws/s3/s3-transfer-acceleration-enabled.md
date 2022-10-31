[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Transfer Acceleration Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Transfer Acceleration Enabled |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures that S3 buckets have transfer acceleration enabled to increase the speed of data transfers. |
| **More Info** | S3 buckets should have transfer acceleration enabled to increase the speed of data transfers in and out of Amazon S3 using AWS edge network. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/transfer-acceleration-examples.html |
| **Recommended Action** | Modify S3 bucket to enable transfer acceleration. |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for S3. </br>
3. Scroll down the left navigation pane and Click on "Buckets".</br> 
4. Select the "Bucket" that needs to add policy to and click on its identifier(name) from the "Bucket name" column.</br>
5. Click on the "Properties" tab on the top menu. </br>
6. Click Edit Transfer acceleration. </br>
7. Select Enable. </br> 
8. Click on the "Save" button to make the necessary changes. </br>
9. Repeat steps 4 - 8 to enable transfer accelaration for other S3 buckets in the region. </br>