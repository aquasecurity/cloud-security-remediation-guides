[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Block Storage / Block Volume Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | Block Volume Restorable |
| **Cloud** | ORACLE |
| **Category** | Block Storage |
| **Description** | Ensures block volumes can be restored to a recent point. |
| **More Info** | Having recent backups on block volumes prevents data loss in the case of a catastrophe. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/blockvolumebackups.htm |
| **Recommended Action** | Ensure block volumes have recent backups to prevent data loss. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Block Volumes" under the "Block Storage." </br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step2.png"/>
3. Click on the "Name" as a link to access to the "Boot Volume" setting.</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step3.png"/>
4. On the "Block Volume Details" page, scroll down and select "Block Volume Backups" udner the "Resources."</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step4.png"/>
5. On the "Block Volume Backups" page, check whether any "Block Volume" backup is there or not which can be restored.</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step5.png"/>
6. Repeat steps number 2 - 5 to check other Block Volumes in the account.</br>
7. Navigate to "Block Volumes" under the "Block Storage" and select the "Block Volumes" option to manually create  the "Block Volume Backup".</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step7.png"/>
8. Click on the "Block Volume Backups" under the Resources and then click on the "Create Block Volume Backup" button at the top.</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step8.png"/>
9. On the "Create Block Volume Backup" page, enter the name for the "Boot Volume Backup" and choose the "Backup Type" and click on the "Create Block Volume Backup" button to make the changes.</br> <img src="/resources/oracle/blockstorage/block-volume-restorable/step9.png"/>
10. Repeat steps number 7 - 9 to determine if Block Volumes can be restored to a recent point.</br>
