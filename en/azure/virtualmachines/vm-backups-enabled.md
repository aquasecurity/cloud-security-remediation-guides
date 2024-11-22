[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Backups Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Backups Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Azure virtual machine backups are enabled. |
| **More Info** | Azure Backup provides independent and isolated backups to guard against unintended destruction of the data on your VMs. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/backup/backup-azure-vms-introduction |
| **Recommended Action** | Enable Azure virtual machine backups. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Backup Center".
3. Select the "Backup Instances" option under "Manage" on the left side menu.
4. Select the "+ Backup" button to initiate the "Start: Configure Backup" form.
5. Select the appropriate "Vault" for use and select "Continue".
6. Adjust the Configure Backup settings based on the needs of your environment.
6. Under "Virtual Machines" add the appropriate virtual machines for backup and select "Enable Backup".