[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Kinesis / Kinesis Data Streams Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Kinesis Data Streams Encrypted |
| **Cloud** | AWS |
| **Category** | Kinesis |
| **Description** | Ensures Kinesis data streams are encrypted using AWS KMS key of desired encryption level |
| **More Info** | Data sent to Kinesis data streams can be encrypted using KMS server-side encryption. Existing streams can be modified to add encryption with minimal overhead. Use customer-managed keys instead in order to gain more granular control over encryption/decryption process. |
| **AWS Link** | https://docs.aws.amazon.com/streams/latest/dev/server-side-encryption.html |
| **Recommended Action** | Enable encryption using desired level for all Kinesis streams |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Kinesis". </br>
3. Under the "Amazon Kinesis dashboard" select a Kinesis stream. </br>
4. Select the "Configuration" tab and scroll down to "Encryption". </br>
5. In Server-side encryption, choose edit. </br>
6. Check "Enable server-side encryption". </br>
7. Select Use customer-managed CMK, then choose Save. </br>
8. Choose the "Customer-managed CMK in KMS" from the dropdown list. </br>
9. Click on the "Save" button to make the necessary changes. On the successful configuration changes, one will get "Successfully updated" message. </br>