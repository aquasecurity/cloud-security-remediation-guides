[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Virtual Machine Boot Diagnostics Enabled
## Quick Info

| | |
|-|-|
| **Plugin Title** | Virtual Machine Boot Diagnostics Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that the VM boot diagnostics is enabled for virtual machines. |
| **More Info** | Boot diagnostics is a debugging feature for Azure virtual machines (VM) that allows diagnosis of VM boot failures. Boot diagnostics enables a user to observe the state of their VM as it is booting up by collecting serial log information and screenshots. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/boot-diagnostics |
| **Recommended Action** | Enable boot diagnostics for all virtual machines. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual Machines".
3. Select the corresponding virtual machine by clicking on the "Name" link.
4. In the left side menu, select "Boot diagnostics" from the Support + troubleshooting options.
5. Select the "Settings" option within the Boot diagnostics section
6. Select "Enable" for the appropriate storage account option based on specific need and save the changes.
7. Repeat steps 3 - 6 for other applicable Virtual machines.