[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Logging |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensures object logging is enabled on storage buckets |
| **More Info** | Storage bucket logging helps maintain an audit trail of access that can be used in the event of a security incident. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/access-logs |
| **Recommended Action** | Bucket Logging can only be enabled by using the Command Line Interface and the log bucket must already be created. Use this command to enable Logging: gsutil logging set on -b gs://[LOG_BUCKET_NAME] -o AccessLog  gs://[BUCKET_NAME] |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option. </br> <img src="/cloud-security-remediation-guides/resources/google/storage/bucket-logging/step2.png">
3. On the "Buckets" page, create the log bucket if you dont have one.</br> <img src="/cloud-security-remediation-guides/resources/google/storage/bucket-logging/step3.png"/>
4. Click on the 'cloud shell' icon on the top left of navigation bar ,as bucket logging can only be enabled by using the Command Line Interface.</br> <img src="/cloud-security-remediation-guides/resources/google/storage/bucket-logging/step4.png>
5. Enter the command gsutil logging set on -b gs://[LOG_BUCKET_NAME] -o AccessLog  gs://[BUCKET_NAME] </br> <img src="/cloud-security-remediation-guides/resources/google/storage/bucket-logging/step5.png>
7. Repeat steps number 4-5 to enable logging to all other buckets in the project.

