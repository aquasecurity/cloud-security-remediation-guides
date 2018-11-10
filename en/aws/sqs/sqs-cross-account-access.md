[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SQS / SQS Cross Account Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQS Cross Account Access |
| **Cloud** | AWS |
| **Category** | SQS |
| **Description** | Ensures SQS policies disallow cross-account access |
| **More Info** | SQS policies should be carefully restricted to prevent publishing or reading from the queue from unexpected sources. Queue policies can be used to limit these privileges. |
| **AWS Link** | http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-creating-custom-policies.html |
| **Recommended Action** | Update the SQS policy to prevent access from external accounts. |

## Detailed Remediation Steps

