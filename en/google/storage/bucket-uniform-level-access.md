[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Storage / Bucket Uniform Level Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Uniform Level Access |
| **Cloud** | GOOGLE |
| **Category** | Storage |
| **Description** | Ensures that uniform level access is enabled on storage buckets. |
| **More Info** | Uniform level access for buckets can be used for managing access in a simple way. It enables us to use other security features like IAM conditions. |
| **GOOGLE Link** | https://cloud.google.com/storage/docs/uniform-bucket-level-access#should-you-use |
| **Recommended Action** | Make sure that storage buckets have uniform level access enabled |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Cloud Storage" to select the "Buckets" option.
3. On the "Buckets" page, select the bucket which needs Uniform Level Access to be enabled, and click on the bucket's name. 
4. Select the Permissions tab near the top of the page.
5. In the text box named Access Control, click the Switch to link. Note that the text box disappears 90 days after you enable uniform bucket-level access.
6. In the pop-up menu that appears, select Uniform or Fine-grained.
7. Click Save.