[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Lifecycle Configured

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Lifecycle Configured |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensure that Cloud Storage buckets are using lifecycle management rules to transition objects between storage classes. |
| **More Info** | Lifecycle management rules allow you to delete buckets at the end of their lifecycle and help optimize your data for storage costs. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/managing-lifecycles |
| **Recommended Action** | Modify storage buckets and configure lifecycle rules. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option.
3. On the "Buckets" page, select the bucket which needs to be enabled, and click on the bucket's name.
4. Click on the Lifecycle tab to open the lifecycle rules page. From here you can add, edit or delete existing rules. 
6. To add a new rule, click Add a Rule.
7. In the page that appears, specify a configuration byselecting the action to take when an object meets the conditions and click Continue.
8. Select the conditions under which an action is taken. Click Continue.
9. Review the changes to be made and then click Create.