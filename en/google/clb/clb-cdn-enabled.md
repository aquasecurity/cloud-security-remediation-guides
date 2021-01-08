[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / CLB / CLB CDN Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CLB CDN Enabled |
| **Cloud** | GOOGLE |
| **Category** | CLB |
| **Description** | Ensures that Cloud CDN is enabled on all load balancers |
| **More Info** | Cloud CDN increases speed and reliability as well as lowers server costs. Enabling CDN on load balancers creates a highly available system and is part of GCP best practices. |
| **GOOGLE Link** | https://cloud.google.com/cdn/docs/quickstart |
| **Recommended Action** | Enable Cloud CDN on all load balancers from the network services console. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Network Services" option under the "NETWORKING" and select the "Load balancing." </br> <img src="/resources/google/clb/clb-cdn-enabled/step2.png"/>
3. On the "Load balancing" page , click on the "Name" as a link option to select the load balancer.</br> <img src="/resources/google/clb/clb-cdn-enabled/step3.png"/>
4. On the "Load balancer details" page, scroll down the page and check the "Cloud CDN" option under the "Backend." If it's set to "disabled" then the selected "Load balancer" cannot creates a highly available system and is part of GCP best practices.</br> <img src="/resources/google/clb/clb-cdn-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to verify other "Load balancers" in the account.</br>
6. Navigate to the "Load balancing" option under the "Netowrk Services" of the "NETWORKING", choose the "load balancer" and click on the "Edit" button at the top.</br> <img src="/resources/google/clb/clb-cdn-enabled/step6.png"/>
7. On the "Edit HTTP(S) load balancer" page, click on the "Backend configuration" option, click on the pencil icon next to the "Bucket/VM" present in the "Backend configuration" page.</br> <img src="/resources/google/clb/clb-cdn-enabled/step7.png"/>
8. On the "Edit back-end bucket" page, click on the checkbox next to the "Enable Cloud CDN" and click on the "Update" button to make the changes.</br> <img src="/resources/google/clb/clb-cdn-enabled/step8.png"/>
9. On the "Edit HTTP(S) load balancer" page, click on the "Update" button to save the changes.</br> <img src="/resources/google/clb/clb-cdn-enabled/step9.png"/>
10. Repeat steps number 6 - 9 to enable Cloud CDN on all load balancers from the network services console.</br>

