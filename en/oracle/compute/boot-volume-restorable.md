[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Boot Volume Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | Boot Volume Restorable |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures boot volumes can be restored to a recent point. |
| **More Info** | Having an active backup ensures that the boot volumes can be restored in the event of a compromised system or hardware failure. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/bootvolumes.htm |
| **Recommended Action** | Ensures boot volumes can be restored to a recent point. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Instances" under the "Compute." </br> <img src="/resources/oracle/compute/boot-volume-restorable/step2.png"/>
3. On the "Instances" page, scroll down and click on the "Boot Volumes" option at the left.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step3.png"/>
4. On the "Boot Volumes" page, click on the "Name" as a link to access the configuration options.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step4.png"/>
5. On the "Boot Volume Details" page, scroll down and click on the "Boot Volume Backups" under the "Resources" section.</br>  <img src="/resources/oracle/compute/boot-volume-restorable/step5.png"/>
6. On the "Boot Volume Backups", check if there is any active "Boot Volume Backup" is available or not.</br>  <img src="/resources/oracle/compute/boot-volume-restorable/step6.png"/>
7. Repeat steps number 2 - 6 to check other volumes in the account.</br>
8. Navigate to "Instances" under the "Compute" and select the "Boot Volumes" option to determine that "Boot Volume" can be restored to a recent point.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step8.png"/>
9. On the "Boot Volume Details" page, scroll down and click on the "Boot Volume Backups" under the "Resources" and click on the "Create Boot Volume Backup" button.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step9.png"/>
10. On the "Create Boot Volume Backup" tab, enter the "Name" for the backup and click on the "Create Boot Volume Backup" button.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step10.png"/>
11. Once the backup is ready then the boot volumes can be restored in the event of a compromised system or hardware failure.</br> <img src="/resources/oracle/compute/boot-volume-restorable/step11.png"/>
12. Repeat steps number 8 - 11 to determine if Boot Volumes can be restored to a recent point.</br>
