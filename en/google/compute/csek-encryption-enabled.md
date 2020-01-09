[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / CSEK Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CSEK Encryption Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures Customer Supplied Encryption Key Encryption is enabled on disks |
| **More Info** | Google encrypts all disks at rest by default. By using CSEK only the users with the key can access the disk. Anyone else, including Google, cannot access the disk data. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/customer-supplied-encryption |
| **Recommended Action** | CSEK can only be configured when creating a disk. Delete the disk and redeploy with CSEK. |

## Detailed Remediation Steps


