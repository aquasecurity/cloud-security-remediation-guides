[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Has Tags |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensure S3 Bucket have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/CostAllocTagging.html |
| **Recommended Action** | Modify S3 buckets and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-has-tags/step3.png"/>
4. Select the "Bucket" for which you want to add "Tags".</br><img src="/resources/aws/s3/s3-bucket-has-tags/step4.png"/>
5. Click on the "Properties" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-has-tags/step5.png"/>
6. On Properties tab scroll down and in "Tags" section Click on "Edit" button.</br><img src="/resources/aws/s3/s3-bucket-has-tags/step6.png"/>
7. On "Edit bucket tagging" page Click on "Add a tag" button and enter tag's key, value and Click "Save Changes".</br><img src="/resources/aws/s3/s3-bucket-has-tags/step7.png"/>