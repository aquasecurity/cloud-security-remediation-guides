[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Kinesis / Kinesis Streams Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Kinesis Streams Encrypted |
| **Cloud** | AWS |
| **Category** | Kinesis |
| **Description** | Ensures Kinesis Streams encryption is enabled |
| **More Info** | Data sent to Kinesis Streams can be encrypted using KMS server-side encryption. Existing streams can be modified to add encryption with minimal overhead. |
| **AWS Link** | https://docs.aws.amazon.com/streams/latest/dev/server-side-encryption.html |
| **Recommended Action** | Enable encryption using KMS for all Kinesis Streams. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "Kinesis". </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step2.png"/>
3. Under the "Amazon Kinesis dashboard" choose "Data Firehose" or "Delivery streams" from the left navigation panel. </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step3.png"/>
4. Select the "Firehose Delivery System" that needs to be verified and click on the "Name" to access the delivery stream.</br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step4.png"/>
5. Select the "Configuration" tab and scroll down to "Amazon S3 destination". Click on the S3 bucket link to check the "Encryption" value.</br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step5.png"/>
6. In the Amazon S3 bucket configuration tab that opens, select "Properties" tab. </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step6.png"/>
7. Scroll down to "Default encryption".and if it's set to "Disabled" then the selected "Firehose Delivery System" data is not encrypted. </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step7.png"/>
8. Click "Edit and on the "Edit default encryption" page select "Enable". </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step8.png"/>
9. Under the "Encryption key type" select "AWS Key Management Service key (SSE-KMS)".  </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step9.png"/>
10. In the "AWS KMS key" section select option "Choose from your AWS KMS keys" and in the "AWS KMS key" select your key from the dropdown.</br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step10.png"/>
11. Select the "Enable" option under "Bucket Key" and click on "Save changes" to enable the encryption.</br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step11.png"/>
12. On the successful configuration changes, one will get "Successfully edited default encryption" message. </br> <img src="/resources/aws/kinesis/kinesis-streams-encrypted/step12.png"/>
13. Repeat steps number 4 and 7 to verify all other "Firehose Delivery System".</br>
11. To enable the "Encryption" on selected "Firehose Delivery System" click on the "Name" to access the delivery stream. Under the "Details" tab click on the "Edit" button to make the changes in "Amazon S3 destination". </br> <img src="/resources/aws/kinesis/kinesis-streams-encrypted/step7.png"/>
12. Click on the "Enable" button next to the "S3 encryption" to enable the encryption. </br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step8.png"/>
13. Choose the "KMS master key" from the dropdown list. Choose either the ("Default( aws/s3 )") KMS key or an AWS KMS Customer Master Key (CMK).</br><img src="/resources/aws/kinesis/kinesis-streams-encrypted/step9.png"/>
14. Click on the "Save" button to make the necessary changes. On the successful configuration changes, one will get "Successfully updated delivery stream" message. </br> <img src="/resources/aws/kinesis/kinesis-streams-encrypted/step10.png"/>
15. Repeat steps number 4 and 7 to verify all other "Firehose Delivery System"..</br>
