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
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/backup/backup-instant-restore-capability |
| **Recommended Action** | Configure virtual machine instant restore backup retention policy to retain backups for desired number of days. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Recovery Services vaults". </br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step2.png"/>
3. After searching the "Recovery Vaults", this screen will appear. From here, click on the vault that you have created.</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step3.png"/>
4. After clicking on the vault, a left sidebar will appear, where you can see the "Manage" section.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step4.png"/>

5. Click on "Backup Policies". On the right side, the list of policies will be displayed. Choose the backup policy linked to your VM. </br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step5.png"/>

6. Under the "Instant Restore" section, locate the field labeled "Retain instant recovery snapshot(s) for [5] Day(s)". Update the number of days according to your desired retention period, and then click the "Update" button to save the changes. </br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step6.png"/>
