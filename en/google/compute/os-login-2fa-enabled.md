[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / OS Login 2FA Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | OS Login 2FA Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Virtual Machines instances have OS logic feature enabled and configured with Two-Factor Authentication. |
| **More Info** | Enable OS login Two-Factor Authentication (2FA) to add an additional security layer to your VM instances. The risk of your VM instances getting attcked is reduced significantly if 2FA is enabled. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/oslogin/setup-two-factor-authentication |
| **Recommended Action** | Set enable-oslogin-2fa to true in custom metadata for the instance. |

## Detailed Remediation Steps

1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option.
3. On the "VM Instances" page, select the VM instance which needs to be verified. 
4. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs `OS Login 2FA` enabled for the project.
5. On the "VM instance details" page, select the "Edit" button at the top.
6. On the "VM instance details - Edit page", scroll down the page and under "Metadata" select add item.
7. Add the key as `enable-oslogin-2fa` and set the value as "TRUE."
8. Click on the "Save" button to make the changes.
9. Navigate to "Metadata" under the "Compute Engine" to add project-wide metadata. 
10. Click on the "Edit" button at the top and add an entry similar to the step 6 for the key and the value and click on the "Save" button to make the changes.