[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Load Balancer HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | Load Balancer HTTPS Only |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Ensures LBs are configured to only accept connections on HTTPS ports. |
| **More Info** | For maximum security, LBs can be configured to only accept HTTPS connections. Standard HTTP connections will be blocked. This should only be done if the client application is configured to query HTTPS directly and not rely on a redirect from HTTP. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Balance/Tasks/managinglisteners.htm |
| **Recommended Action** | Remove non-HTTPS listeners from load balancer. |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Load Balancers" under the "Networking." </br> <img src="/resources/oracle/networking/load-balancer-https-only/step2.png"/>
3. On the "Load Balancers" page, select the "Load Balancer" by clicking on the "Name" as a link to access the "Load Balancer."</br>  <img src="/resources/oracle/networking/load-balancer-https-only/step3.png"/>
4. On the "Load Balancer Details" page, scroll down and select "Listeners" under the "Resources".</br> <img src="/resources/oracle/networking/load-balancer-https-only/step4.png"/>
5. Check if there is any non-HTTPS listeners attached with the "Load balancer". Non-HTTPS listeners are not suggested as best practices under GCP.</br> <img src="/resources/oracle/networking/load-balancer-https-only/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Load balancer" in the accounts.</br>
7. Navigate to "Load balancers" under the "Networking", click on the "Name" as a link to access the "Load balancer" which needs to modify the "Listeners" attached.</br> <img src="/resources/oracle/networking/load-balancer-https-only/step7.png"/>
8. Click on the "Listners" option under the "Resources" to remove any non-HTTPS lister.</br> <img src="/resources/oracle/networking/load-balancer-https-only/step8.png"/>
9. Click on the 3dots at the extreme right to open the "Options" tab and click on the "Delete" option to remove the non-HTTPS listener.</br> <img src="/resources/oracle/networking/load-balancer-https-only/step9.png"/>
10. On the "Delete Listener" tab, click on the "Delete" button to make the changes.</br> <img src="/resources/oracle/networking/load-balancer-https-only/step10.png"/>
11. Create a HTTPS listeners and attached the SSL's as per the company policy.</br>
12. Repeat steps number 7 - 10 to remove non-HTTPS listeners from load balancer.</br>
