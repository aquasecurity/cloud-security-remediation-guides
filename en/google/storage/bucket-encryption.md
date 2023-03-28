[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Uniform Level Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Uniform Level Access |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensure that Cloud Storage buckets have encryption enabled using desired protection level. |
| **More Info** | By default, all storage buckets are encrypted using Google-managed keys. To have better control over how your storage bucktes are encrypted, you can use Customer-Managed Keys (CMKs). |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/encryption/customer-managed-keys |
| **Recommended Action** | Ensure that all storage buckets have desired encryption level. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option.
3. On the "Buckets" page, select the bucket by clicking on the bucket's name. 
4. In the bucket details page, click on the Configuration tab.
5. Click on the Pencil icon associated with the Encryption type entry.
6. Set or remove the default Cloud KMS key for the bucket.
    a. If the bucket isn't currently using a Cloud KMS key, select the Customer-managed key radio button, then select one of the available keys in the associated drop-down menu.
    b. If the bucket currently uses a Cloud KMS key, change the Cloud KMS key in the drop-down menu by selecting the Google-managed key radio button.

7. Click Save.