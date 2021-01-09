[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Block Storage / Block Volume Backup Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Block Volume Backup Enabled |
| **Cloud** | ORACLE |
| **Category** | Block Storage |
| **Description** | Ensures block volumes have backups enabled. |
| **More Info** | Enabling block volume backup policies ensures that the block volume can be restored following in the event of data loss. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/blockvolumebackups.htm |
| **Recommended Action** | Enable backups on each block volume. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Block Volumes" under the "Block Storage." </br> <img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step2.png"/>
3. Click on the "Name" as a link to access to the "Boot Volume" setting.</br> <img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step3.png"/>
4. On the "Block Volume Details" page, scroll down and check on the left whether "Backup Policy" is enabled or not.</br> <img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to check other Block Volumes in the account.</br>
6. Navigate to "Block Volumes" under the "Block Storage" and select the "Block Volumes" option to enable the "Block Volume Backup".</br> <img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step6.png"/>
7. On the "Block Volume Details" page, click on the "Assign" option next to the "Backup Policy."</br><img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step7.png"/>
8. On the "Assign Backup Policy" page, select the "Backup Policy" type from the dropdown menu as per the requirements and click on the "Assign" button to make the changes.</br> <img src="/resources/oracle/blockstorage/block-volume-backup-enabled/step8.png"/>
9. Repeat steps number 6 - 8 to enable "Block Volumes Backup."</br>

