[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Object Write Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Object Write Logging |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensure that Object-level logging for write events is enabled for S3 bucket. |
| **More Info** | Enabling Object-level S3 event logging significantly enhances security, especially for sensitive data. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/enable-cloudtrail-logging-for-s3.html#enable-cloudtrail-events |
| **Recommended Action** | Enable object level logging for Write events for each S3 bucket. |

## Detailed Remediation Steps
**Note**
To configure a trail to log data events for an S3 bucket, you can use either the AWS CloudTrail console or the Amazon S3 console. If you are configuring a trail to log data events for all the Amazon S3 buckets in your AWS account, it's easier to use the [CloudTrail console](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-data-events-with-cloudtrail.html#logging-data-events).

The following steps shows how to use the Amazon S3 console to configure a CloudTrail trail to log data events for an S3 bucket.

1. Sign in to the AWS Management Console and open the [Amazon S3 console](https://console.aws.amazon.com/s3/).
2. In the Buckets list, choose the name of the bucket.</br> <img src="/resources/aws/s3/s3-object-write-logging/step2.png"/>
3. Choose Properties.</br> <img src="/resources/aws/s3/s3-object-write-logging/step3.png"/>
4. Under AWS CloudTrail data events, choose Configure in CloudTrail.</br> <img src="/resources/aws/s3/s3-object-write-logging/step4.png"/>
5. You can create a new CloudTrail trail or reuse an existing trail and configure Amazon S3 data events to be logged in your trail. For information about how to create trails in the CloudTrail console, see [Creating and updating a trail with the console](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-data-events-with-cloudtrail.html#logging-data-events). For information about how to configure Amazon S3 data event logging in the CloudTrail console, see [Logging data events for Amazon S3 Objects](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-data-events-with-cloudtrail.html#logging-data-events-examples).

**Note**
Additional charges apply for data events. For more information, see [AWS CloudTrail pricing](https://aws.amazon.com/cloudtrail/pricing/).