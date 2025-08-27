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

1. Log in to the Microsoft Azure Management Console.

2. In the search bar at the top, select Search resources, services, and docs and search for "Recovery Services vaults".
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step2.png"/>

3. In the search results for "Recovery Vaults", select the vault you have created.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step3.png"/>

4. After selecting the vault, a left sidebar will appear. Locate the Manage section.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step4.png"/>

5. Click on Backup Policies. The list of policies will appear on the right. Select the backup policy linked to your VM. If no policy is available, click the Add icon to create a new backup policy.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step5.png"/>

6. When creating a new policy, select Azure Virtual Machine as the policy type.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step6.png"/>

7. Choose Enhanced, provide a name for the policy, and then click Create.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step7.png"/>

8. After successfully creating the policy, click on it to modify the Instant Restore settings.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step8.png"/>

9. The Instant Restore value will be displayed (default is 7 days). If you require more instant restore days, edit the field and click Update.
</br> <img src="/resources/azure/virtualmachines/vm-instant-restore-backup-retention-period/step9.png"/>
