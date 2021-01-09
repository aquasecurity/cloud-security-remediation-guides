[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Boot Volume Backup Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Boot Volume Backup Enabled |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures boot volumes have a backup policy. |
| **More Info** | Enabling a boot volume backup policy ensures that the boot volumes can be restored in the event of a compromised system or hardware failure. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/bootvolumes.htm |
| **Recommended Action** | Ensure all boot volumes have a backup policy. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Instances" under the "Compute." </br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step2.png"/>
3. On the "Instances" page, scroll down and click on the "Boot Volumes" option at the left.</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step3.png"/>
4. On the "Boot Volumes" page, click on the "Name" as a link to access the configuration options.</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step4.png"/>
5. On the "Boot Volume Details" page, scroll down and check on the left whether "Backup Policy" is enabled or not.</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other volumes in the account.</br>
7. Navigate to "Instances" under the "Compute" and select the "Boot Volumes" option to enable the "Boot Volume Backup".</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step7.png"/> 
8. On the "Boot Volume Details" page, click on the "Assign" option next to the "Backup Policy."</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step8.png"/>
9. On the "Assign Backup Policy" page, select the "Backup Policy" type from the dropdown menu as per the requirements and click on the "Assign" button to make the changes.</br> <img src="/resources/oracle/compute/boot-volume-backup-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to enable backup policy in Boot Volumes.
