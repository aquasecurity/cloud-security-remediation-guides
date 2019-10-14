[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Storage Bucket All Users Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Bucket All Users Policy |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensures Storage bucket policies do not allow global write, delete, or read permissions |
| **More Info** | Storage buckets can be configured to allow the global principal to access the bucket via the bucket policy. This policy should be restricted only to known users or accounts. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/access-control/iam |
| **Recommended Action** | 1. Enter the Storage Service. 2. Select the ... next to the Bucket and choose Edit Bucket Permissions. 3. In each Permission, ensure that no member is allUsers or allAuthenticatedUsers  |

## Detailed Remediation Steps

