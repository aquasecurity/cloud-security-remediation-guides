[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SQS / SQS Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQS Has Tags |
| **Cloud** | AWS |
| **Category** | SQS |
| **Description** | Ensures that Amazon SQS queue has tags associated |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-queue-tags.html |
| **Recommended Action** | Update SQS queue and add tags. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for SQS. </br> <img src="/resources/aws/sqs/sqs-has-tags/step2.png"/>
3. Select the "SQS" queue that needs to be verified by clicking on its "Name".</br> <img src="/resources/aws/sqs/sqs-has-tags/step3.png"/>
4. Scroll down the page and click on the "Tagging" tab from the bottom panel. And click Edit button</br> <img src="/resources/aws/sqs/sqs-has-tags/step4.png"/>
5. Scroll to the bottom of the page and click on "Add new tag" button. And Enter key and value for tag then, click on "Save" button. </br> <img src="/resources/aws/sqs/sqs-has-tags/step5.png"/>
6. Repeat steps number 3 - 5 to ensure tags on remaining SQS queues</br>
