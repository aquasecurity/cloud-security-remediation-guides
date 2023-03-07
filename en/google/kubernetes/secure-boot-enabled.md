[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Secure Boot Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Secure Boot Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes cluster nodes have secure boot feature enabled. |
| **More Info** | Secure Boot feature protects your cluster nodes from malware and makes sure the system runs only authentic software. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/shielded-gke-nodes#secure_boot |
| **Recommended Action** | Ensure that Secure Boot feature is enabled for all node pools in your GKE clusters. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under "Compute" and select the "Clusters." 
3. On the "Kubernetes clusters" page, click the name of the cluster you want to modify.
4. Click + Add Node Pool.
5. From the navigation menu, click Security.
6. Under Shielded options, select the Enable secure boot checkbox.
    - Note that Secure boot is a node pool setting that's disabled by default on GKE because third-party unsigned kernel modules cannot be loaded when secure boot is enabled. If you don't use third-party unsigned kernel modules, you can enable secure boot.
7. Click Create
8. Repeat steps 3 - 7 for all other applicable clusters.