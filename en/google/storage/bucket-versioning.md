[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Versioning

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Versioning |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensures object versioning is enabled on storage buckets |
| **More Info** | Object versioning can help protect against the overwriting of objects or data loss in the event of a compromise. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/using-object-versioning |
| **Recommended Action** | Bucket Versioning can only be enabled by using the Command Line Interface, use this command to enable Versioning: gsutil versioning set on gs://[BUCKET_NAME] |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Click on the 'cloud shell' icon on the top left of navigation bar ,as Bucket Versioning can only be enabled by using the CLI (Command Line Interface) .</br> <img src="/resources/google/storage/bucket-versioning/step2.png"/>
3. Enter the command gsutil versioning set on gs://[BUCKET_NAME] </br> <img src="/resources/google/storage/bucket-versioning/step3.png"/>
4. Repeat steps 3 to enable versioning to all other buckets in the project.
