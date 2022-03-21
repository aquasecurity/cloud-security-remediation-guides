[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SQS / SQS Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQS Encrypted |
| **Cloud** | AWS |
| **Category** | SQS |
| **Description** | Ensures SQS encryption is enabled |
| **More Info** | Messages sent to SQS queues can be encrypted using KMS server-side encryption. Existing queues can be modified to add encryption with minimal overhead. |
| **AWS Link** | http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-server-side-encryption.html |
| **Recommended Action** | Enable encryption using KMS for all SQS queues. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for SQS. </br> <img src="/resources/aws/sqs/sqs-encrypted/step2.png"/>
3. Select the "SQS" queue that needs to be verified and click on its "Name".</br> <img src="/resources/aws/sqs/sqs-encrypted/step3.png"/>
4. Scroll down the page and click on the "Encryption" tab from the bottom panel.</br> <img src="/resources/aws/sqs/sqs-encrypted/step4.png"/>
5. Check the "Server Side Encryption" status for the selected "SQS" queue. If the "Server Side Encryption" is not configured then the following message is  displayed "No server-side encryption is set for this queue". SSE protects the content of messages in Amazon SQS queues using keys managed in the AWS Key Management Service (AWS KMS)".</br> <img src="/resources/aws/sqs/sqs-encrypted/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQS" queue in the selected AWS region.</br>
7. To enable the "SQS" encryption navigate to KMS services to create a "KMS CMK customer-managed key".</br> <img src="/resources/aws/sqs/sqs-encrypted/step7.png"/>
8. Scroll down the left navigation panel and choose "Customer managed keys" under "Key Management Service" and click on the "Create key" button at the top panel.</br> <img src="/resources/aws/sqs/sqs-encrypted/step8.png"/>
9. On the "Configure key" page select key type as "Symmetric". In the advanced options select "Key material origin" as "KMS" and "Regionality" as "Single-Region key" and proceed by clicking "Next" button.</br> <img src="/resources/aws/sqs/sqs-encrypted/step9.png"/>
10. On the "Add labels" page provide the "Alias" and "Description" for the new "KMS key" and click on the "Next" button. You can define unique tags for  "Tag key", "Tag value" under the "Tags" section. </br> <img src="/resources/aws/sqs/sqs-encrypted/step10.png"/>
11. On the "Define key administrative permissions" page select the "IAM users" and roles who can administer the new "KMS key" through the KMS API and click "Next" button.</br> <img src="/resources/aws/sqs/sqs-encrypted/step11.png"/>
12. On the "Define key usage permissions" page select the IAM users and roles that can use the CMK to encrypt and decrypt SQS data with the "AWS KMS API" and click on the "Next" button.</br> <img src="/resources/aws/sqs/sqs-encrypted/step12.png"/>
13. On the "Review" page review the policy and click on the "Finish" button to create a new "KMS key" which can be used to encrypt/decrypt the SQS data.</br> <img src="/resources/aws/sqs/sqs-encrypted/step13.png"/>
14. Now "KMS CMK customer-managed key" is created navigate to SQS and select the "SQS" queue which needs to be modified and click the "Edit" button at the top.</br> <img src="/resources/aws/sqs/sqs-encrypted/step14.png"/>
15. On the "Edit TestQueue" page scroll down to "Encryption" and under the "Server-Side Encryption" select "Enabled". </br> <img src="/resources/aws/sqs/sqs-encrypted/step15.png"/>
16. Under the "Encryption key type" select "AWS Key Management Service key (SSE-KMS)" and from the dropdown under "Customer master key" select the key that you have created for SQS.</br> <img src="/resources/aws/sqs/sqs-encrypted/step16.png"/>
17. Click on the "Save" button to make the necessary changes.</br> <img src="/resources/aws/sqs/sqs-encrypted/step17.png"/>
18. Repeat steps number 7 - 17 to enable encryption using KMS for all SQS queues.</br>
