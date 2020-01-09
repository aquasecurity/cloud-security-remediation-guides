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


