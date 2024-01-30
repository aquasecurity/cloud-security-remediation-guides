[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Pub/Sub / Topic Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Topic Encryption Enabled |
| **Cloud** | GOOGLE |
| **Category** | Pub/Sub |
| **Description** | Ensure that Google Pub/Sub topics are encrypted with desired encryption level. |
| **More Info** |Google encrypts all messages in topics by default. By using CSEK, only the users with the key can access the disk. Anyone else, including Google, cannot access the disk data. |
| **GOOGLE Link** | https://cloud.google.com/pubsub/docs/encryption |
| **Recommended Action** | Ensure that Cloud Pub/Sub topics are encrypted using CSEK keys. |

## Detailed Remediation Steps
You can configure CMEK using the Google Cloud console or the gcloud command-line tool. For prerequisites, you must have:
1. Created a key ring and a regional or global key in Cloud KMS. Keys and key rings cannot be deleted.
2. Enabled the Cloud KMS API.
You can use the Google Cloud console topic creation dialog to add your encryption keys: </br> <img src="/resources/google/pubsub/topic-encryption-enabled/step1.png">
To verify that Pub/Sub topic are not encrypted using a Customer-Managed Key (CMK) follow these steps:
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Pub/Sub".
3. Select Topics to access the Pub/Sub topics created for the selected GCP project.
4. Click on the identifier (ID) of the topic that you want to examine.
5. In the Topic details section, check the Encryption key configuration attribute value. If the Encryption key attribute value is set to Google-managed key, the messages published to the selected Google Cloud Pub/Sub topic are not encrypted using a Customer-Managed Key (CMK).
6. Repeat step no. 4 and 5 for each Pub/Sub topic created within the selected project.
7. 7Repeat steps no. 2 – 6 for each project deployed within your Google Cloud account.