[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Scale Sets Boot Diagnostics Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets Boot Diagnostics Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that boot diagnostics is enabled for Virtual Machine Scale Set. |
| **More Info** | Boot diagnostics is a debugging feature for Azure virtual machines (VM) scale sets that allows diagnosis of VM scale set boot failures. Boot diagnostics enables a user to observe the state of their scale set as it is booting up by collecting serial log information and screenshots. |
| **AZURE Link** | https://learn.microsoft.com/en-us/troubleshoot/azure/virtual-machines/boot-diagnostics |
| **Recommended Action** | Enable boot diagnostics for virtual machine scale set. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. Once the scale set is selected, navigate to "Monitoring" > "Boot diagnostics".
5. Under Boot diagnostics settings, ensure "Enable with managed storage account" is selected.
6. Repeat steps 3-5 for all applicable scale set instances.