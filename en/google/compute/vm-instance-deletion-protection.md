[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Instance Deletion Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instance Deletion Protection |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Virtual Machine instances have deletion protection enabled. |
| **More Info** | VM instances should have deletion protection enabled in order to prevent them for being accidentally deleted. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/preventing-accidental-vm-deletion |
| **Recommended Action** | Modify VM instances to enable deletion protection |

## Detailed Remediation Steps
1.  Go to the VM instances page.

    [Go to VM instances](https://console.cloud.google.com/compute/instances)

2.  If prompted, select your project and click Continue.

3.  Click the name of the instance for which you want to toggle deletion protection. The instance details page displays.

4.  From the instance details page, complete the following steps:

    a.  Click the Edit button at the top of the page.
    b.  Under Deletion Protection, check the box to enable or uncheck the box to disable deletion protection.
    c.  Save your changes.