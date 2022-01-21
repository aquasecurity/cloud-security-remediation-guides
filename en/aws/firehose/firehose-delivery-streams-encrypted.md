[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Firehose / Firehose Delivery Streams Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Firehose Delivery Streams Encrypted |
| **Cloud** | AWS |
| **Category** | Firehose |
| **Description** | Ensures Firehose Delivery Stream encryption is enabled |
| **More Info** | Data sent through Firehose Delivery Streams can be encrypted using KMS server-side encryption. Existing delivery streams can be modified to add encryption with minimal overhead. |
| **AWS Link** | https://docs.aws.amazon.com/firehose/latest/dev/encryption.html |
| **Recommended Action** | Enable encryption using KMS for all Firehose Delivery Streams. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "Kinesis". </br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step2.png"/>
3. Under the "Amazon Kinesis dashboard" choose "Data Firehose" or "Delivery streams" from the left navigation panel. </br><img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step3.png"/>
4. Select the "Firehose Delivery System" that needs to be verified and click on the "Name" to access the delivery stream.</br><img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step4.png"/>
5. Select the "Configuration" tab and scroll down to "Server-side encryption (SSE)" and if it's set to "Disabled" then the selected "Firehose Delivery System" data is not encrypted. </br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step5.png"/>
6. Enable the "Encryption" on selected "Firehose Delivery System" by clicking on the "Edit" button.</br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step6.png"/>
7. Select "Enable server-side encryption for source records in delivery stream" under "Server-side encryption". </br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step7.png"/>
8. Under "Encryption type" select "Use AWS owned CMK" if you want to create a new customer managed key for encryption. </br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step8.png"/>
9. If you already have your own encryption key then select "Use customer managed CMK" under "Encryption type" and select the existing key.</br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step9.png"/>
10. Click on the "Save" button to make the necessary changes. On the successful configuration changes, one will get "Successfully updated delivery stream" message. </br> <img src="/resources/aws/firehose/firehose-delivery-streams-encrypted/step10.png"/>
12. Repeat steps number 4 to 10 to verify all other "Firehose Delivery streams".</br>
