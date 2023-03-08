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
| **GOOGLE Link** | https://cloud.google.com/storage/docs/bucket-lock?_ga=2.221806616.-1645770163.1613190642 |
| **Recommended Action** | Modify bucket to configure retention policy and lock retention policy. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option.
3. On the "Buckets" page, select the bucket which needs to be enabled, and click on the bucket's name.
4. Select the Protection tab near the top of the page.
5. In the Retention policy section, set your retention policy:
  - If no retention policy currently applies to the bucket, click the + Set Retention Policy link. Choose a unit of time and a length of time for your retention period.
  - If a retention policy currently applies to a bucket, it appears in the section. Click Edit to modify the retention time.
6. To set a lock on the retention policy, click the Lock button.
7. Upon clicking the Lock button, a Lock retention policy dialog box will appear. Read the Permanent notice. 
8. In the Bucket name text box, type in the name of your bucket.
9. Click Lock policy.