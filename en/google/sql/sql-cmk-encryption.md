[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SQL CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL CMK Encryption |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Intended for organizations that have sensitive or regulated data that requires them to manage their own encryption keys. |
| **More Info** | The CMEK feature lets you use your own cryptographic keys for data at rest in Cloud SQL. After adding customer-managed encryption keys, whenever an API call is made, Cloud SQL uses your key to access data. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/create-manage-users |
| **Recommended Action** | Use default encryption keys. |

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the Cloud Storage Buckets page.

    [Go to Buckets](https://console.cloud.google.com/storage/browser)

2.  In the list of buckets, click on the desired bucket.

3.  In the bucket details page, click on the Configuration tab.

4.  Click on the Pencil icon associated with the Encryption type entry.

5.  Set or remove the default Cloud KMS key for the bucket.

    a.  If the bucket isn't currently using a Cloud KMS key, select the Customer-managed key radio button, then select one of the available keys in the associated drop-down menu.

    b.  If the bucket currently uses a Cloud KMS key, change the Cloud KMS key in the drop-down menu, or remove the Cloud KMS key by selecting the Google-managed key radio button.

6.  Click Save.

To learn how to get detailed error information about failed Cloud Storage operations in the Google Cloud console, see [Troubleshooting](https://cloud.google.com/storage/docs/troubleshooting#trouble-console).