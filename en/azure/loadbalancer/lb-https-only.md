[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Load Balancer / LB HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | LB HTTPS Only |
| **Cloud** | AZURE |
| **Category** | Load Balancer |
| **Description** | Ensures load balancers are configured to only accept connections on HTTPS ports |
| **More Info** | For maximum security, load balancers can be configured to only accept HTTPS connections. Standard HTTP connections will be blocked. This should only be done if the client application is configured to query HTTPS directly and not rely on a redirect from HTTP. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-overview |
| **Recommended Action** | Ensure that each load balancer only accepts connections on port 443. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Load balancers. </br> <img src="/resources/azure/loadbalancer/lb-https-only/step2.png"/>
3. Select the "Load balancer" by clicking on the "Name" as a link which needs to be configured only to accept connections on HTTPS ports. </br> <img src="/resources/azure/loadbalancer/lb-https-only/step3.png"/>
4. On the "load balancer" page, scroll down the left navigation panel and choose the "Load balancing rules" option under "Settings".</br> <img src="/resources/azure/loadbalancer/lb-https-only/step4.png"/>
5. On the "Load balancing rules" page if the "Load balancing rule" is showing as "TCP/80" then the selected "Load balancer" is configured to accept connections on HTTP ports.</br> <img src="/resources/azure/loadbalancer/lb-https-only/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Load balancers" in the account.</br>
7. Navigate to "Load Balancer", select the "Load balancer" by clicking on the "Name" as a link, scroll down the left navigation panel and choose "Load balancing rule."</br> <img src="/resources/azure/loadbalancer/lb-https-only/step7.png"/>
8. On the "Load balancing rule" page click on the "Name" as a link to access the configuration changes.</br> <img src="/resources/azure/loadbalancer/lb-https-only/step8.png"/>
9. Scroll down the "Load balancing rule" page and select the "Port" and "Backend Port" as 443 and save the changes.</br> <img src="/resources/azure/loadbalancer/lb-https-only/step9.png"/>
10. Repeat the steps number 7 - 9 to ensure that each load balancer only accepts connections on port 443.</br>

