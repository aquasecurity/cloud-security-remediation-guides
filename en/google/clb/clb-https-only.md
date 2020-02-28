[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / CLB / CLB HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | CLB HTTPS Only |
| **Cloud** | GOOGLE |
| **Category** | CLB |
| **Description** | Ensures CLBs are configured to only accept connections on HTTPS ports |
| **More Info** | For maximum security, CLBs can be configured to only accept HTTPS connections. Standard HTTP connections will be blocked. This should only be done if the client application is configured to query HTTPS directly and not rely on a redirect from HTTP. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/vpc |
| **Recommended Action** | Remove non-HTTPS listeners from the load balancer. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Network Services" option under the "NETWORKING" and select the "Load balancing." </br> <img src="/resources/google/clb/clb-https-only/step2.png"/>
3. On the "Load balancing" page , click on the "Name" as a link option to select the load balancer.</br> <img src="/resources/google/clb/clb-https-only/step3.png"/>
4. On the "Load balancer details" page, scroll down the page and check the "Protocol" option under the "Fronend." If it's set to "HTTP" then the selected "Load balancer" is not a part of GCP best practices.</br> <img src="/resources/google/clb/clb-https-only/step4.png"/>
5. Repeat steps number 2 - 4 to verify other "Load balancers" in the account.</br>
6. Navigate to the "Load balancing" option under the "Netowrk Services" of the "NETWORKING", choose the "load balancer" and click on the "Edit" button at the top.</br> <img src="/resources/google/clb/clb-https-only/step6.png"/>
7. On the "Edit HTTP(S) load balancer" page, click on the "Frontend configuration" option, click on the pencil icon next to the "Bucket/VM" present in the "Frontend configuration" page.</br> <img src="/resources/google/clb/clb-https-only/step7.png"/>
8. On the "Frontend configuration" tab, select the "Protocol" as "HTTPS" and select the corresponding certificate and click on the "Done" button.</br> <img src="/resources/google/clb/clb-https-only/step8.png"/>
9. On the "Edit HTTP(S) load balancer" page, click on the "Update" button to save the changes.</br> <img src="/resources/google/clb/clb-https-only/step9.png"/>
10. Repeat steps number 6 - 9 to remove non-HTTPS listeners from the load balancer.

