[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Daily Backup Retention Period

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Daily Backup Retention Period |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that VM daily backup retention policy is configured to retain backups for the desired number of days. |
| **More Info** | Azure Backup provides independent and isolated backups to guard against unintended destruction of the data on your VMs. These backups should be retained for a specific amount of time to recover destroyed VM.|
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/backup/backup-azure-vms-introduction |
| **Recommended Action** | Configure virtual machine daily backup retention policy to retain backups for desired number of days. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Backup Center".
3. Select the "Backup Policies" option under "Manage" by clicking on the "Name" link to access the configuration changes. 
4. In the selected "Policy" under the "Retention Range" section, select "Retention of daily backup point" and set the time and days to the desired retention amount. Save the changes. 
5. Note that a minimum of 5 days is suggested for audit compliance.
6. Repeat steps number 3 - 4 to verify other "Policies" in the Backup Center.
