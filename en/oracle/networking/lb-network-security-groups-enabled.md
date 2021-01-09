[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / LB Network Security Groups Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | LB Network Security Groups Enabled |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Ensures Load Balancers are using network security groups to restrict network access. |
| **More Info** | Network security groups gives fine grained control of resources. Security rules associated with network security groups can be associated with specific resources. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/networking_security.htm |
| **Recommended Action** | Ensure Load Balancers are using network security groups to restrict network access. |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Load Balancers" under the "Networking." </br> <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step2.png"/>
3. On the "Load Balancers" page, select the "Load Balancer" by clicking on the "Name" as a link to access the "Load Balancer."</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step3.png"/>
4. On the "Load Balancer Details" page, scroll down and click on the "Network Security Group" attached.</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step4.png"/>
5. On the "Security Rules" page, check which ports are opened under "Ingress Rules" and check only specific traffic ports based on requirement is allowed.</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "LB Network Security Groups" in the account.</br>
7. Navigate to "Load balancers" under the "Networking", click on the "Name" as a link to access the "Load balancer" which needs to modify the "Network Security Group" attached.</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step7.png"/>
8. On the "Load Balancer Details" page, click on the "Edit" button next to "Network Security Group" to make the changes.</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step8.png"/>
9. On the "Edit Network Security Groups" tab, select the "best Network Security Group" for the load balancer and click on the "Save Changes" button.</br>  <img src="/resources/oracle/networking/lb-network-security-groups-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure Load Balancers are using Network Security Groups to restrict network access.</br>
