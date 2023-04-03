[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Shielded Nodes

## Quick Info

| | |
|-|-|
| **Plugin Title** | Shielded Nodes |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensure that shielded nodes setting is enabled for all Kubernetes clusters. |
| **More Info** | Shielded GKE nodes give strong cryptographic identity. This prevents attackers from being able to impersonate a node in your GKE cluster even if the attacker can extract the node credentials. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/shielded-gke-nodes |
| **Recommended Action** | Ensure that shielded nodes setting is enabled in your GKE cluster. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under "Compute" and select the "Clusters."
3. Click the name of the cluster you want to modify.
4. Under Security, in the Shielded GKE Nodes field, click edit Edit Shielded GKE Nodes.
5. Select the Enable Shielded GKE Nodes checkbox.
6. Click Save Changes
7. Repeat steps 3 - 6 for all other applicable clusters.