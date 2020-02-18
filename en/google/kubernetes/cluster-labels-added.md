[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Cluster Labels Added

## Quick Info

| | |
|-|-|
| **Plugin Title** | Cluster Labels Added |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes clusters have labels added |
| **More Info** | It is recommended to add labels to Kubernetes clusters to apply specific security settings and auto configure objects at creation. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/creating-managing-labels |
| **Recommended Action** | Ensure labels are added to Kubernetes clusters |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/cluster-labels-added/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/cluster-labels-added/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/cluster-labels-added/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Labels" are added or not. If "Lables" are showing "None" then specific security settings and auto configure objects at creation cannot be done. <img src="/resources/google/kubernetes/cluster-labels-added/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/cluster-labels-added/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and click on the "Add label" and add as per the requirement.</br> <img src="/resources/google/kubernetes/cluster-labels-added/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/cluster-labels-added/step9.png"/>
10. Repeat steps number 7 - 9 to ensure labels are added to Kubernetes clusters.</br>
