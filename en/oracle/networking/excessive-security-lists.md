[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Excessive Security Lists

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Security Lists |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Determine if there are an excessive number of security lists in the account |
| **More Info** | Keeping the number of security lists to a minimum helps reduce the attack surface of an account. Rather than creating new groups with the same rules for each project, common rules should be grouped under the same security lists. For example, instead of adding port 22 from a known IP to every group, create a single "SSH" security group which can be used on multiple instances. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Network/Concepts/securitylists.htm |
| **Recommended Action** | Limit the number of security lists to prevent accidental authorizations |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Virtual Cloud Networks" under the "Networking." </br> <img src="/resources/oracle/networking/excessive-security-lists/step2.png"/>
3. On the "Virtual Cloud Networks" page, click on the "Name" as a link to access the "Virtual Network." </br> <img src="/resources/oracle/networking/excessive-security-lists/step3.png"/>
4. On the "Virtual Cloud Network Details" page, scroll down the left navigation panel and choose the "Security Lists" option under the "Resources." </br> <img src="/resources/oracle/networking/excessive-security-lists/step4.png"/>
5. On the "Security Lists" page, check the number of "Security Lists" and check if multiple security list is serving the same traffic rules by clicking on the "Name" as a link.</br> <img src="/resources/oracle/networking/excessive-security-lists/step5.png"/>
6. Repeat steps number 2 - 5 to determine if there are an excessive number of security lists in the account which serves the same traffic rules.</br>
7. Navigate to "Virtual Cloud Networks" under the "Networking", click on the "Name" as a link to access the "Virtual Network", select the "Security List" which needs to be removed.</br> <img src="/resources/oracle/networking/excessive-security-lists/step7.png"/>
8. Click on the 3 vertical dots at the extreme right of the screen to open the "Options" window of the selected "Security List."</br> <img src="/resources/oracle/networking/excessive-security-lists/step8.png"/>
9. Click on the "Terminate" at the bottom of the "Options" window and click on the "Yes" button at the "Terminate Security List" tab.</br> <img src="/resources/oracle/networking/excessive-security-lists/step9.png"/>
10. Repeat steps number 7 - 9 to limit the number of security lists to prevent accidental authorizations.</br>
