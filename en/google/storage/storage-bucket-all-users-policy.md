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
| **Recommended Action** | Ensure that each storage bucket is configured so that no member is set to allUsers or allAuthenticatedUsers. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option. </br> <img src="/resources/google/storage/storage-bucket-all-users-policy/step2.png">
3. On the "Buckets" page, select the bucket which you want to configure by clicking on the checkbox next to its name.</br> <img src="/resources/google/storage/bstorage-bucket-all-users-policy/step3.png"/>
4. Select the "PERMISSIONS" tab to access the permissions defined for selected bucket.</br> <img src="/resources/google/storage/storage-bucket-all-users-policy/step4.png"/>
5. Select the "VIEW BY PRINCIPALS" tab to display all IAM members (principals) that have access to the selected resource.. </br> <img src="/resources/google/storage/storage-bucket-all-users-policy/step5.png"/>
6. Select all the allUsers and allAuthenticatedUsers principals available and choose REMOVE ACCESS to initiate the removal action for the selected bindings.</br><img src="/resources/google/storage/storage-bucket-all-users-policy/step6.png"/>
7. On the removal confirmation box, choose "CONFIRM" to remove the allUsers and/or allAuthenticatedUsers principals.</br> <img src="/resources/google/storage/storage-bucket-all-users-policy/step7.png"/>
8. Repeat steps number 4-7 to remove all allUsers or allAuthenticatedUsers access from all other buckets in the project.</br>

