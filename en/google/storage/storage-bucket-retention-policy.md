[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Storage Bucket Retention Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Bucket Retention Policy |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensures bucket retention policy is set and locked to prevent deleting or updating of bucket objects or retention policy. |
| **More Info** | Configuring retention policy for bucket prevents accidental deletion as well as modification of bucket objects. This retention policy should also be locked to prevent policy deletion. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/bucket-lock?_ga=2.221806616.-1645770163.1613190642|
| **Recommended Action** | Modify bucket to configure retention policy and lock retention policy. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option. </br> <img src="/resources/google/storage/bucket-retention-policy/step2.png">
3. On the "Buckets" page, select the bucket which you want to configure by clicking on its name.</br> <img src="/resources/google/storage/bucket-retention-policy/step3.png"/>
4. Select the "PROTECTION" tab to access the protection configuration defined for selected bucket.</br> <img src="/resources/google/storage/bucket-retention-policy/step4.png"/>
5. Scroll down to "Bucket retention policy" configuration and click on "SET RETENTION POLICY" to add the retention policy to the selected bucket</br> <img src="/resources/google/storage/bucket-retention-policy/step5.png"/>
6. A popup panel will appear, select the desired retention period and click on "save" to save the retention policy.</br> <img src="/resources/google/storage/bucket-retention-policy/step6.png"/>
7. Repeat steps number 4-6 to add retention policy to all other buckets in the project.</br>
