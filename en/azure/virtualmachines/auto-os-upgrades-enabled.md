[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Automatic OS Upgrades Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Automatic OS Upgrades Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensure that automatic operating system (OS) upgrades are enabled for Microsoft Azure virtual machine scale sets. |
| **More Info** | Enabling automatic OS image upgrades on your scale set helps ease update management by safely and automatically upgrading the OS disk for all instances in the scale set. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-automatic-upgrade |
| **Recommended Action** | Enable automatic OS upgrades under operating system settings. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. Once the scale set is selected, select "Upgrade policy" in the left side menu under Settings.
5. Select "Automatic" in the drop down menu for "Upgrade Mode" and save the changes.
6. Repeat steps 3-5 for all applicable scale set instances.