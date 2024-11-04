[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Has Tags |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensure that AWS S3 Bucket have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/CostAllocTagging.html |
| **Recommended Action** | Modify S3 buckets and add tags. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console and open the Amazon [S3 console](https://console.aws.amazon.com/s3/).
2. In the Buckets list, choose the name of the bucket that you want to view the properties for.</br> <img src="/resources/aws/s3/s3-bucket-has-tags/step2.png"/>
3. Choose the Properties tab.</br> <img src="/resources/aws/s3/s3-bucket-has-tags/step3.png"/>
4. On the Properties page, scroll down to tags, and click Edit.</br> <img src="/resources/aws/s3/s3-bucket-has-tags/step4.png"/>
5. Click Add tag, and fill in the information.</br> <img src="/resources/aws/s3/s3-bucket-has-tags/step5.png"/>
6. Click Save changes. 