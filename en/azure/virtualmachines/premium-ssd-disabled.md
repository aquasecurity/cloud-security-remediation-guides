[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Premium SSD Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Premium SSD Disabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that the Azure virtual machines are configured to use standard SSD disk volumes instead of premium SSD disk volumes for managed disks. |
| **More Info** | Azure standard SSD disks store data on solid state drives (SSDs), like Azure's existing premium storage disks. Standard SSD disks are a cost-effective storage option optimized for workloads that need consistent performance at lower IOPS levels. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/disks-types |
| **Recommended Action** | Modify virtual machines disks to use standard SSD disk volumes instead of premium SSD disk volumes. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines.
3. Select the Virtual Machine instance to modify by clicking on the "Name" link
4. Select "Disks" on the left menu side menu settings and then select the appropriate disk by clicking on the "Disk name" link.
5. Select "Side + Performanmce" on the left menu side menu settings.
6. Select "Standard SSD (locally-redundant storage" under "Disk SKU"
7. Select the disk size appropriate for the needs of your environment and then select "Resize" to apply the changes.