[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Open All Ports Protocols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open All Ports Protocols |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Determine if security list has all ports or protocols open to the public |
| **More Info** | Security lists should be created on a per-service basis and avoid allowing all ports or protocols. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Network/Concepts/securitylists.htm |
| **Recommended Action** | Modify the security list to specify a specific port and protocol to allow. |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Virtual Cloud Networks" under the "Networking." </br> <img src="/resources/oracle/networking/open-all-ports-protocols/step2.png"/>
3. On the "Virtual Cloud Networks" page, click on the "Name" as a link to access the "Virtual Network." </br> <img src="/resources/oracle/networking/open-all-ports-protocols/step3.png"/>
4. On the "Virtual Cloud Network Details" page, scroll down the left navigation panel and choose the "Network Security Groups" option under the "Resources." </br> <img src="/resources/oracle/networking/open-all-ports-protocols/step4.png"/>
5. On the "Network Security Groups" page, select the "Security group" by clicking on the "Name" as a link to access the security group.</br> <img src="/resources/oracle/networking/open-all-ports-protocols/step5.png"/>
6. On the "Network Security Group Details" page, under the "Security Rules" check if security list has all ports or protocols open to the public. </br> <img src="/resources/oracle/networking/open-all-ports-protocols/step6.png"/>
7. Repeat steps number 2 - 6 to check other "Security Groups" in the account.</br>
8. Navigate to "Virtual Cloud Networks" under the "Networking", click on the "Name" as a link to access the "Virtual Network", select the "Security Group" in which security list has all ports or protocols open to the public.</br> <img src="/resources/oracle/networking/open-all-ports-protocols/step8.png"/>
9. On the "Security Rules" page, click on the checkbox of the "Ingress" and click on the "Edit" button at the top to make the changes.</br> <img src="/resources/oracle/networking/open-all-ports-protocols/step9.png"/>
10. On the "Edit Rules" page, enter the "IP Address" as per requirements under the "Source CIDR" and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/networking/open-all-ports-protocols/step10.png"/>
11. Repeat steps number to restrict security list to specify a specific port and protocol to allow. </br>
