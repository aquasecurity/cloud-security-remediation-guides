[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Lifecycle Configured

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Lifecycle Configured |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensure that Cloud Storage buckets are using lifecycle management rules to transition objects between storage classes. |
| **More Info** | Lifecycle management rules allow you to delete buckets at the end of their lifecycle and help optimize your data for storage costs.|
| **GOOGLE Link** | https://cloud.google.com/storage/docs/managing-lifecycles |
| **Recommended Action** | Modify storage buckets and configure lifecycle rules. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option. </br> <img src="/resources/google/storage/bucket-lifecycle-configured/step2.png">
3. On the "Buckets" page, select the bucket which needs to be configured with lifycyvle rules by clicking on the "name".</br> <img src="/resources/google/storage/bucket-lifecycle-configured/step3.png"/>
4. Select the "LIFECYCLE" tab to access the lifecycle configuration defined for selected bucket.</br> <img src="/resources/google/storage/bucket-lifecycle-configured/step4.png"/>
5. Click on "ADD A RULE" to add the rule for lifecycle configuration. </br> <img src="/resources/google/storage/bucket-lifecycle-configured/step5.png"/>
6. Select the desire action and create the rule. Click on "CREATE" button to add the rule.</br> <img src="/resources/google/storage/bucket-lifecycle-configured/step6.png"/>
7. Repeat steps number 4-6 to configure encryption of lifecycle rules to all other buckets in the project.</br>
