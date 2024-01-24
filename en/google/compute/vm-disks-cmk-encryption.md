[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Disks CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Disks CMK Encryption |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Virtual Machine instances are encrypted using customer-managed keys. |
| **More Info** | Google encrypts all disks at rest by default. By using CMKs you can have better control over your disk encryption. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/customer-supplied-encryption |
| **Recommended Action** | Ensure that your VM instances have CMK encryption enabled.  |

## Detailed Remediation Steps
1. Log in to the [GCP Console](https://console.cloud.google.com). </br>
2. Navigate to VM instances.</br><img src="/resources/google/compute/vm-disks-cmk-encryption/step2.png"/></br>
3. In the Instance detail page, click the instance name.</br>
4. Click Edit.</br><img src="/resources/google/compute/vm-disks-cmk-encryption/step4.png"/></br>
5. In the Boot disk and Additional disks sections, check the encryption type available in the Encryption column for each disk attached to the instance. If the selected disk does not have the Encryption type set to Customer managed, the data on the verified disk is not encrypted with a Customer-Managed Key (CMK), therefore the disk(s) attached to your Google Compute Engine instance are not encrypted with CMKs.
