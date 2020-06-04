[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Block Storage / Volume Groups Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | Volume Groups Restorable |
| **Cloud** | ORACLE |
| **Category** | Block Storage |
| **Description** | Determine if Volume Groups can be restored to a recent point. |
| **More Info** | Enabling Volume Groups backups ensures that the volume group can be restored following in the event of data loss. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/volumegroups.htm |
| **Recommended Action** | 1. Enter the Volume Groups Service. 2. Select the Volume Group in question. 3. Select the backups blade on the lower left side. 4. Create a backup. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Volume Groups" under the "Block Storage." </br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step2.png"/>
3. Click on the "Name" as a link to access to the "Volume Group" settings.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step3.png"/>
4. On the "Volume Group Details" page, scroll down and select the "Volume Groups Backup" blade on the lower left side.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step4.png"/>
5. On the "Volume Group Backups", check if there is any "Volume Group Backup" is available or not which can be restored to a recent point.</br> <img src="/resources/oracle/blockstorage/volume-groups-restorable/step5.png"/>
6. Repeat steps number 2 - 4 to check other Volume Groups in the account.</br>
