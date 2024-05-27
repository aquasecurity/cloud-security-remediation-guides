[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | BBucket Encryption |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensure that Cloud Storage buckets have encryption enabled using desired protection level. |
| **More Info** | By default, all storage buckets are encrypted using Google-managed keys. To have better control over how your storage bucktes are encrypted, you can use Customer-Managed Keys (CMKs). |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/encryption/customer-managed-keys |
| **Recommended Action** | Ensure that all storage buckets have desired encryption level. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option. </br> <img src="/resources/google/storage/bucket-encryption/step2.png">
3. On the "Buckets" page, select the bucket which needs to be configured with the desire encryption level by clicking on the checkbox next to its name.</br> <img src="/resources/google/storage/bucket-encryption/step3.png"/>
4. Select the "CONFIGURATION" tab to access the configuration defined for selected bucket.</br> <img src="/resources/google/storage/bucket-encryption/step4.png"/>
5. Select on Encryption type and click on edit option. </br> <img src="/resources/google/storage/bucket-encryption/step5.png"/>
5. A popup panel will appear on screen.</br>
6. Select the desire encryption level want to set on selected bucket and then click "Save" </br> <img src="/resources/google/storage/bucket-encryption/step7.png"/>
7. Repeat steps number 4-6 to configure encryption of desire level to all other buckets in the project.</br>
