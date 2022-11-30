[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / No Empty Scale Sets

## Quick Info

| | |
|-|-|
| **Plugin Title** | No Empty Scale Sets |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that virtual machine scale sets have virtual machine instances attached. |
| **More Info** | Azure virtual machine scale sets let you create and manage a group of load balanced VMs. Scale sets with no vm instances should be deleted to save cost of unused resources. |
| **AZURE Link** | Delete virtual machine scale sets that have no virtual machine instances. |
| **Recommended Action** | https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets"
3. Select a scale set by clicking on the "Name" link
4. Once open, in the "Overview" section, select "Move" to link the scale set to a virtual machine. 
5. Repeat steps 3-4 for all other scale sets.
6. See https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/quick-create-portal if no scale sets are present.