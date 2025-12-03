[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Instant Restore Backup Retention Period

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instant Restore Backup Retention Period |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that VM instant restore backup retention policy is configured to retain backups for the desired number of days. |
| **More Info** | Azure Backup provides independent and isolated backups to guard against unintended destruction of the data on your VMs. These backups should be retained for a specific amount of time to recover destroyed VM. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/backup/backup-instant-restore-capability |
| **Recommended Action** | Configure virtual machine instant restore backup retention policy to retain backups for desired number of days. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Backup Center.
3. Select "Backup Policies" under the Manage section.
4. Select the policy impacting the at risk Virtual Machine by clicking on the "Name" link.
5. In the Modify Policy form, change the "Retain instant recovery snapshot(s) for" number of days to five(5) or greater and then click Save.
6. Apply these changes to all applicable policies.