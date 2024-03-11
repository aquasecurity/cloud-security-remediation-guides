[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Integrity Monitoring Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Integrity Monitoring Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes shielded cluster node have integrity monitoring enabled |
| **More Info** | Integrity Monitoring feature automatically monitors the integrity of your cluster nodes. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/shielded-gke-nodes#integrity_monitoring |
| **Recommended Action** | Enable Integrity Monitoring feature for your cluster nodes |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under "Compute" and select the "Clusters." 
3. On the "Kubernetes clusters" page, click the name of the cluster you want to modify.
4. Click + Add Node Pool.
5. From the navigation menu, click Security.
6. Under Shielded options, select the Enable integrity monitoring checkbox.
7. Click Create
8. Repeat steps 3 - 7 for all other applicable clusters.