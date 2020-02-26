[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Network Policy Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Network Policy Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes clusters have network policy enabled |
| **More Info** | Kubernetes network policy creates isolation between cluster pods, this creates a more secure environment with only specified connections allowed. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/network-policy |
| **Recommended Action** | Enable network policy on all Kubernetes clusters. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/network-policy-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/network-policy-enabled/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/network-policy-enabled/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Network policy for master" is enabled or disabled. If it's set to disabled then it's not as per the best recommended method.</br> <img src="/resources/google/kubernetes/network-policy-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/network-policy-enabled/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and choose the "Enabled" option from the dropdown menu next to "Network policy for master."</br> <img src="/resources/google/kubernetes/network-policy-enabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/network-policy-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to enable network policy on all Kubernetes clusters. </br>


