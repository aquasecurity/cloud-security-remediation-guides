[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Managed VM Machine Image

## Quick Info

| | |
|-|-|
| **Plugin Title** | Managed VM Machine Image |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that VM is launched from a managed VM image. |
| **More Info** | A managed VM image contains the information necessary to create a VM, including the OS and data disks. Virtual Machines should be launched using managed images to ensure security practices and consistency across all the instances. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/windows/create-vm-generalized-managed |
| **Recommended Action** | Ensure that VM is launched using managed VM image. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines.
3. Select the applicable Virtual Machine from the list of Virtual Machines by clicking on the "name" link.
4. In the left side menu for the Virtual Machine, select "Disks" under Settings.
5. At the top of the Disks section, select "Migrate to managed disks".
6. If your VM is in an availability set, there will be a warning on the Migrate to managed disks blade that you need to convert the availability set first. The warning should have a link you can click to convert the availability set. Once the availability set is converted or if your VM is not in an availability set, click Migrate to start the process of migrating your disks to managed disks.
7. The VM will be stopped and restarted after migration is complete.
8. Repeat steps 3-5 for all other applicable disks.