[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for SQS. </br> <img src="/resources/aws/sqs/sqs-cross-account-access/step2.png"/>
3. Select the "SQS" queue that needs to be verify from "Name".</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step3.png"/>
4. Scroll down the page and click on the "Permissions" tab from the bottom panel.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step4.png"/>
5. Check the "Principals" column under "Permissions" and if "Everyobdy" or "AWS Account ID" which does not match any of the trusted AWS account than the selected "SQS" queue cross-account access is not secured.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQS" queues in the selected AWS region.</br>
7. Navigate to "SQS" and choose "SQS" queue that needs to modify to secure the cross-account access and select the "Permissions" tab from the bottom panel. </br> <img src="/resources/aws/sqs/sqs-cross-account-access/step7.png"/>
8. Click on the pencil icon in the "Permissions" tab to edit the selected "SQS" queue permission.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step8.png"/>
9. In the "Add a Permission" dialog box click on the "Deny" option under the "Effect" to explicitly deny permission to the untrusted AWS account ID's and click on the "Save" button to make the necessary changes.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step9.png"/>
10. Repeat steps number 7 - 9 to update the SQS policy to prevent access from external accounts.</br>
