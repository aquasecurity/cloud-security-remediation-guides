[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Scale Sets Health Monitoring Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets Health Monitoring Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that health monitoring is enabled for virtual machine scale sets. |
| **More Info** | Scale set health monitoring feature reports on VM health from inside the scale set instance and can be configured to probe on an application endpoint and update the status of the application on that instance. That instance status is checked by Azure to determine whether an instance is eligible for upgrade operations. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-health-extension |
| **Recommended Action** | Enable health monitoring for virtual machine scale sets. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets"
3. Select on the corresponding scale set by clicking on the "Name" link.
4. In the left side pane, select "Health and repair" under Settings.
5. Enable the application health monitoring and enable automatic repairs. Save the changes.
6. Restart the scale set for the changes to take effect. 
7. Repeat steps 3 - 6 for any other applicable scale sets.