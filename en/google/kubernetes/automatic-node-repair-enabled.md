[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Automatic Node Repair Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Automatic Node Repair Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes cluster nodes have automatic repair enabled |
| **More Info** | When automatic repair on nodes is enabled, the Kubernetes engine performs health checks on all nodes, automatically repairing nodes that fail health checks. This ensures that the Kubernetes environment stays optimal. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-repair |
| **Recommended Action** | Ensure that automatic node repair is enabled on all node pools in Kubernetes clusters |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step3.png"/>
4. On the selected "Clusters" page, scroll down and select the "Node pools" by clicking on the "Name" as a link.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step4.png"/>
5. On the "Node pool details" page, scroll down the page, check "Auto-repair" option under the "Management" and if it's showing "Disabled" then the Kubernetes engine cannot perform health checks on all nodes.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other clusters in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and select the "Node pools" option.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step7.png"/>
8. On the "Node pool details" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step8.png"/>
9. On the "Edit node pool" page, scroll down and click on the checkbox next to the "Enable auto-repair" under the "Management."</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/automatic-node-repair-enabled/step10.png"/>
11. Repeat steps number 7 - 10 to ensure that automatic node repair is enabled on all node pools in Kubernetes clusters.</br>
