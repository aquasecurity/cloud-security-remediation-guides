[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine / Old VM Disk Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | Old VM Disk Snapshots |
| **Cloud** | AZURE |
| **Category** | Virtual Machine |
| **Description** | Ensures that virtual machines do not have older disk snapshots. |
| **More Info** | A snapshot is a full, read-only copy of a virtual hard drive (VHD). You can take a snapshot of an OS or data disk VHD to use as a backup, or to troubleshoot virtual machine (VM) issues. VM snapshots older than a specific period of time should be deleted to save cost of unused resources. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/windows/snapshot-copy-managed-disk |
| **Recommended Action** | Ensure that there are no undesired old VM disk snapshots. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Snapshots".
3. Select the applicable Snapshot by clicking on the "Name" link.
4. In the left menu pane, select "Snapshot export" if applicable and export a version of the snapshot if required to keep.
5. Select the "Overview" menu section and click on "Delete" to remove the snapshot from the environment. 
6. Repeat steps 3 - 5 for any other applicable snapshots.