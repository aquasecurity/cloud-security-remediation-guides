[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Default Security List

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default Security List |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Ensure the default security lists block all traffic by default |
| **More Info** | The default security list is often used for resources launched without a defined security list. For this reason, the default rules should be to block all traffic to prevent an accidental exposure. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Network/Concepts/securitylists.htm |
| **Recommended Action** | Update the rules for the default security list to deny all traffic by default |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Virtual Cloud Networks" under the "Networking." </br> <img src="/resources/oracle/networking/default-security-list/step2.png"/>
3. On the "Virtual Cloud Networks" page, click on the "Name" as a link to access the "Virtual Network." </br> <img src="/resources/oracle/networking/default-security-list/step3.png"/>
4. On the "Virtual Cloud Network Details" page, scroll down the left navigation panel and choose the "Security Lists" option under the "Resources." </br> <img src="/resources/oracle/networking/default-security-list/step4.png"/>
5. On the "Security Lists" page, click on the "Name" as a link for "Default Security List" to access the security list.</br> <img src="/resources/oracle/networking/default-security-list/step5.png"/>
6. On the "Default Security List" check if there are any ports open for traffic. If yes, then it's not as per the best practices define by GCP.</br> <img src="/resources/oracle/networking/default-security-list/step6.png"/>
7. Repeat steps number 2 - 6 to verify "Default Security Group" in other accounts.</br>
8. Navigate to "Virtual Cloud Networks" under the "Networking", click on the "Name" as a link to access the "Virtual Network", select the "Default Security List" which needs to block all traffic by default.</br> <img src="/resources/oracle/networking/default-security-list/step8.png"/>
9. On the "Default Security List" page, select the "Ingress Rules" and click on the "Remove" button at the top to remove any "Ingress Traffic rule."</br> <img src="/resources/oracle/networking/default-security-list/step9.png"/>
10. Repeat "Step 9" for the "Egress Rules."</br> <img src="/resources/oracle/networking/default-security-list/step10.png"/>
11. Repeat steps number 8 - 10 to update the rules for the default security list to deny all traffic by default.</br>
