[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Block Storage / Volume Groups Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | Volume Groups Restorable |
| **Cloud** | ORACLE |
| **Category** | Block Storage |
| **Description** | Ensures volume groups can be restored to a recent point. |
| **More Info** | Enabling volume groups backups ensures that the volume group can be restored following in the event of data loss. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/volumegroups.htm |
| **Recommended Action** | Ensure volume groups can be restored to a recent point. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Volume Groups" under the "Block Storage." </br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step2.png"/>
3. Click on the "Name" as a link to access to the "Volume Group" settings.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step3.png"/>
4. On the "Volume Group Details" page, scroll down and select the "Volume Groups Backup" blade on the lower left side.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step4.png"/>
5. On the "Volume Group Backups", check if there is any "Volume Group Backup" is available or not which can be restored to a recent point.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step5.png"/>
6. Repeat steps number 2 - 4 to check other Volume Groups in the account.</br>
7. Navigate to "Group Volumes" under the "Block Storage" and select the "Group Volumes" option to manually create  the "Volume Group Backup".</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step7.png"/>
8. Click on the "Volume Group Backups" under the Resources and then click on the "Create Volume Group Backup" button at the top.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step8.png"/>
9. On the "Create Volume Group Backup", enter the name for the "Volume Group Backup" and choose the "Backup Type" and click on the "Create" button to make the changes.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step9.png"/>
10. Repeat steps number 7 - 9 to determine if Volume Groups can be restored to a recent point.</br>
