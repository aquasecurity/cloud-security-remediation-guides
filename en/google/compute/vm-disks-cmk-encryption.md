[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Disks CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Disks CMK Encryption |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Encrypt a new persistent disk with CSEK |
| **More Info** | By default, Compute Engine encrypts all data at rest. However, if you want to control and manage this encryption yourself, you can provide your own encryption keys. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/customer-supplied-encryption |
| **Recommended Action** | Encrypt a new persistent disk by supplying a key during VM or disk creation.  |

## Detailed Remediation Steps
1.  Go to the Images page.

    [Go to Images](https://console.cloud.google.com/compute/images)

2.  Click Create image.

3.  Under Source disk, choose the encrypted disk you want to create an image of.

4.  Under Encryption, select an encryption key management solution.

5.  If the key has been wrapped with the public RSA key, select Wrapped key.