[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Health Monitoring Extension HTTPS Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Health Monitoring Extension HTTPS Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that Virtual Machine Scale Set has HTTPS enabled for health monitoring. |
| **More Info** | Enabling Application Health Extension in Virtual Machine Scale Set instance reports on application health from inside based on HTTPS responses received from the application. This allows to initiate repairs on unhealthy instances and to determine if an instance is eligible for upgrade operations. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-health-extension |
| **Recommended Action** | Modify virtual machine scale set extensions and enable HTTPS for health monitoring.|

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. Once the scale set is selected, select "Extensions + Applications".
5. Look for an extension named ApplicationHealthWindows (for Windows) or ApplicationHealthLinux (for Linux) and choose the appropriate extension.
6. Repeat steps 3-5 for all applicable scale set instances.