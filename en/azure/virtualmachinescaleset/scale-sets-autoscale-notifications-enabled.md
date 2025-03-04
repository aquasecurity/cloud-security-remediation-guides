[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Scale Sets Autoscale Notifications Enabled
## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets Autoscale Notifications Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that Virtual Machine scale sets have autoscale notifications enabled. |
| **More Info** | Autoscale automatically creates new instances when certain metrics are surpassed, or can destroy instances that are being underutilized. Autoscale notifications should be enabled to know about the status of autoscale operation.|
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-monitor/autoscale/autoscale-overview |
| **Recommended Action** | Ensure that autoscale notifications are enabled for all Virtual Machine Scale Sets. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding virtual machine scale set by clicking on the "Name" link. 
4. In the left side menu, select "Scaling" from the Settings section.
5. In the Scaling section, select the "Notify" option.
6. In the Notify section, check the appropriate notification box for either administrators or co-administrators and save the changes.
7. Repeat steps 3 - 6 for all other applicable virtual machine scale sets.