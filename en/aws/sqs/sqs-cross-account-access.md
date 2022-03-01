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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for SQS. </br> <img src="/resources/aws/sqs/sqs-cross-account-access/step2.png"/>
3. Select the "SQS" queue that needs to be verified by clicking on its "Name".</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step3.png"/>
4. Scroll down the page and click on the "Access Policy" tab from the bottom panel.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step4.png"/>
5. Check the "Principal" key under "Access policy (Permissions)" and if set to "*" or an "AWS Account ID" which does not match any of the trusted AWS accounts then the selected "SQS" queue cross-account access is not secured.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step5.png"/>
6. To edit the selected "SQS" queue permission click on "Edit button.  </br> <img src="/resources/aws/sqs/sqs-cross-account-access/step6.png"/>
7. On the "Edit Queue" page scroll down to "Access policy" and change the "Principle" value from Everyone(*) to relevant AWS Account Id ( e.g. { "AWS": "arn:aws:iam::102604298007:role/aws-elasticbeanstalk-ec2-role" } ) of the AWS account.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step7.png"/>
8. Click on the "Save" button to make the necessary changes.</br> <img src="/resources/aws/sqs/sqs-cross-account-access/step8.png"/>
9. Repeat steps number 3 - 8 to update the SQS policy to prevent access from external accounts.</br>
