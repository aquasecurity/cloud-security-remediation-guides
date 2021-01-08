[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Private Cluster Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Private Cluster Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures private cluster is enabled for all Kubernetes clusters |
| **More Info** | Kubernetes private clusters only have internal ip ranges, which ensures that their workloads are isolated from the public internet. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/private-clusters |
| **Recommended Action** | Ensure that all Kubernetes clusters have private cluster enabled. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/private-cluster-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/private-cluster-enabled/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/private-cluster-enabled/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Private cluster" is enabled or disabled. If it's set to disabled then it's not as per the best recommended method. </br> <img src="/resources/google/kubernetes/private-cluster-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/private-cluster-enabled/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and choose the "Enabled" option from the dropdown menu next to "Private cluster."</br> <img src="/resources/google/kubernetes/private-cluster-enabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/private-cluster-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that all Kubernetes clusters have private cluster enabled.</br>

