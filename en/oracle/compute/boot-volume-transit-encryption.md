[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Boot Volume Transit Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Boot Volume Transit Encryption |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures in-transit data encryption is enabled on boot volumes. |
| **More Info** | Enabling boot volume in-transit data encryption ensures that boot volume data is secured and follows Oracle security best practices. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Block/Concepts/bootvolumes.htm |
| **Recommended Action** | boot volume transit encryption can only be configured when creating a new instance. Recreate the instance with in-transit encryption enabled. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Instances" under the "Compute." </br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step2.png"/>
3. On the "Instances" page, scroll down and click on the "Boot Volumes" option at the left.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step3.png"/>
4. On the "Boot Volumes" page, click on the "Name" as a link to access the configuration options.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step4.png"/>
5. On the "Boot Volume Details" page, scroll down and select "Attached Instances" under the "Resources".</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step5.png"/>
6. In the "Attached Instances", check "In-Transit Encryption" is enabled or not.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step6.png"/>
7. Repeat steps number 2 - 6 to verify other volumes in the account.</br>
8. Navigate to "Instances" under the "Compute" and select the "Boot Volumes" option to enable the "Boot Volume Transit Encryption".</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step8.png"/>
9. On the "Boot Volume" page, scroll down and choose the "Boot Volume Clones" under the "Resources".</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step9.png"/>
10. On the "Boot Volume Clones" page, click on the 3dots at the extreme right and choose the "Create Instance" option.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step10.png"/>
11. On the "Create Compute Instance" page, scroll down and click on the "Show Shape, Network and Storage Options" to expand the services.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step11.png"/>
12. On the expand services under "Shape, Network and Storage Options", scroll down and select the checkbox next to the "USE IN-TRANSIT ENCRYPTION" under the "Boot Volume" and click on the "Create" button to initiate a new Instance.</br> <img src="/resources/oracle/compute/boot-volume-transit-encryption/step12.png"/>
13. Repeat steps number 8 - 12 to enable in-transit data encryption.</br>
