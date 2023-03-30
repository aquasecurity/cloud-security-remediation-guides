[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Deprecated Images

## Quick Info

| | |
|-|-|
| **Plugin Title** | Deprecated Images |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Compute instances are not created from deprecated images. |
| **More Info** | Deprecated Compute Disk Images should not be used to create VM instances. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/images/image-management-best-practices |
| **Recommended Action** | Ensure that no compute instances are created from deprecated images. |

## Detailed Remediation Steps
1. To deprecate an existing image, log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Compute Engine" to select the "Images" option.
3. For the image you want to deprecate, click &#8942; &#x22EE; &vellip; Actions.
4. Select Deprecate.
5. For state, select either Deprecated or Obsolete.
6. Specify a replacement image.
7. Click Deprecate Image.

## Optional
1. Delete the deprecated image by checking the box to the left of the image you want to delete.
2. Click Delete at the top of the page. Your image is now deleted.