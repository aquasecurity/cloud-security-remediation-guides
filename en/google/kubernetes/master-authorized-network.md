[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Master Authorized Network

## Quick Info

| | |
|-|-|
| **Plugin Title** | Master Authorized Network |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures master authorized networks is set to enabled on Kubernetes clusters |
| **More Info** | Authorized networks are a way of specifying a restricted range of IP addresses that are permitted to access your container clusters Kubernetes master endpoint. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/authorized-networks |
| **Recommended Action** | Enable master authorized networks on all clusters. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/master-authorized-network/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/master-authorized-network/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/master-authorized-network/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Master authorised networks" is enabled or disabled. If it's set to disabled then it's not as per the best recommended method to authenticate.</br> <img src="/resources/google/kubernetes/master-authorized-network/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/master-authorized-network/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and choose the "Enabled" option from the dropdown menu next to "Master authorised networks."</br> <img src="/resources/google/kubernetes/master-authorized-network/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/master-authorized-network/step9.png"/>
10. Repeat steps number 7 - 9 to enable master authorized networks on all clusters.</br>

