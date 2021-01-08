[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Automatic Node Upgrades Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Automatic Node Upgrades Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes cluster nodes have automatic upgrades enabled |
| **More Info** | Enabling automatic upgrades on nodes ensures that each node stays current with the latest version of the master branch, also ensuring that the latest security patches are installed to provide the most secure environment. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-upgrades |
| **Recommended Action** | Ensure that automatic node upgrades are enabled on all node pools in Kubernetes clusters |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step3.png"/>
4. On the selected "Clusters" page, scroll down and select the "Node pools" by clicking on the "Name" as a link.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step4.png"/>
5. On the "Node pool details" page, scroll down the page, check "Auto-upgrade" option under the "Management" and if it's showing "Disabled" then it doesn't ensures that each node stays current with the latest version of the master branch.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other clusters in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and select the "Node pools" option.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step7.png"/>
8. On the "Node pool details" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step8.png"/>
9. On the "Edit node pool" page, scroll down and click on the checkbox next to the "Enable auto-upgrade" under the "Management."</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/automatic-node-upgrades-enabled/step10.png"/>
11. Repeat steps number 7 - 10 to ensure automatic node upgrades are enabled on all node pools in Kubernetes clusters.</br>


