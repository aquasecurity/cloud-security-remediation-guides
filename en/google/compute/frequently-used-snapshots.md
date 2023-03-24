[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Frequently Used Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | Frequently Used Snapshots |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that frequently used disks are created from images instead of snapshots to save networking cost. |
| **More Info** | If you are repeatedly using a snapshot in the same zone to create a persistent disk, save networking costs by using the snapshot once and creating an image of that snapshot. Store this image and use it to create your disk and start a VM instance. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/snapshot-best-practices#prepare_for_consistency |
| **Recommended Action** | Ensure that your disk snapshots have images created from them. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. In the left navigation panel choose "Compute Engine" and then select the "Create an Image" option.
3. Specify the Name of your image.
4. Specify the Source from which you want to create an image by selecting a snapshot.
5. In the Based on source disk location (default) drop-down list, specify the location to store the image. If you don't make a selection, Compute Engine stores the image in the multi-region closest to your image's source location.
6. Optional: specify the properties for your image.
7. Specify the encryption key. You can choose between a Google-managed key, a Cloud Key Management Service (Cloud KMS) key or a customer- supplied encryption (CSEK) key. If no encryption key is specified, images are encrypted using a Google-managed key.
8. Click Create to create the image.

**These configuration changes may incur additional costs**