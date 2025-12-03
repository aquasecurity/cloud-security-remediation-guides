[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Automatic Instance Repairs Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Automatic Instance Repairs Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that automatic instance repairs is enabled for Azure virtual machine scale sets. |
| **More Info** | Enabling automatic instance repairs for Azure virtual machine scale sets helps achieve high availability for applications by maintaining a set of healthy instances. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-automatic-instance-repairs |
| **Recommended Action** | Enable automatic instance repairs for Azure virtual machine scale sets. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the scale set by clicking on the "Name" link.
4. Select "Health and Repair" in the left hand menu under Settings.
5. Select "Enabled" in Enable application health monitoring.
6. Select "On" for Enable automatic repairs. Note that the "Health" extension will need to be added to the Virtual Machines associated with this scale set and the scale set may need restarted prior to the changes successfully being made.
7. Save the changes.
8. Repeat steps 3-7 for all other scale sets.