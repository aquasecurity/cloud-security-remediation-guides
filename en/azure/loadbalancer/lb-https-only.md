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
2. In the search bar at the top search for Load balancers and select the "Load balancer" from the results. </br> <img src="/resources/azure/loadbalancer/lb-https-only/step2.png"/>
3. Select the "Load balancer" by clicking on the "Name" link that needs to be configured to accept HTTPS connections only. </br> <img src="/resources/azure/loadbalancer/lb-https-only/step3.png"/>
4. On the "load balancer" page, scroll down the left navigation panel and choose the "Load balancing rules" option under "Settings".</br> <img src="/resources/azure/loadbalancer/lb-https-only/step4.png"/>
5. On the "Load balancing rules" page if the "Load balancing rule" is showing as "TCP/80" then the selected "Load balancer" is configured to accept connections on HTTP ports.</br> <img src="/resources/azure/loadbalancer/lb-https-only/step5.png"/>
6. Click on the triple dots (...) at the end of HTTP rule row and click on "Delete".</br> <img src="/resources/azure/loadbalancer/lb-https-only/step6.png"/>
7. Click "Yes" in the confirmation box that opens.</br> <img src="/resources/azure/loadbalancer/lb-https-only/step7.png"/>
8. Repeat the steps number 3 - 7 to ensure that each load balancer only accepts HTTPS connections on port 443.</br>

