[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Disks / Unmanaged Disk Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unmanaged Disk Encryption |
| **Cloud** | AZURE |
| **Category** | Disks |
| **Description** | Ensures that unmanaged disks are encrypted |
| **More Info** | Encrypting unmanaged data disks (non-boot volume) ensures that the entire contents are fully unrecoverable without a key, protecting the volume from unwarranted reads. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-apply-disk-encryption |
| **Recommended Action** | Enable Data Disk Encryption on all unmanaged disks |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step2.png"/>
3. On the "Security Center" page, scroll down the left navigation panel and choose "Recommnedations" under the "RESOURCE SECURITY HYGIENE."</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step3.png"/>
4. On the "Security Center - Recommendations" page if the "Disk encryption should be applied on virtual machines" is under the "Recommendations" then there is no protecting the volume from unwarranted reads.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step4.png"/>
5. Repeat steps number 2 - 4 to check other "Security Recommendations." </br>
6. Navigate to "Security Center", scroll down the left  navigation panel and choose the "Recommnedations" and under the "Security Center - Recommendations" page follow the instructions to apply encryption to these VMs.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step6.png"/>
7. On the "Security Center - Recommendations Disk encryption should be applied on virtual machines", scroll down the page and under the "Remediation steps" click on the "Encryption Instructions" link.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step7.png"/>
8. On the "Security Center" page, scroll down the left navigation panel and choose the "Security Policy" under the "POLICY & COMPLIANCE."</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step8.png"/>
9. On the "Security Policy" page, click on the name of the subscription that needs to reconfigure.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step9.png"/>
10. On the "Security policy" page select the "ASC Default" policy assignment to edit the subscription configuration settings.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step10.png"/>
11. On the selected policy assignment scroll down the page and "select AuditIfNotExists" from "Monitor disk encryption" dropdown list to enable disk encryption monitoring under "Parameters."</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step11.png"/>
12. Scroll down the page and click on the "Assign" button to make the changes.</br> <img src="/resources/azure/disks/unmanaged-disk-encryption/step12.png"/>
13. Repeat steps number 6 - 12 to enable Data Disk Encryption on all unmanaged disks.</br>
