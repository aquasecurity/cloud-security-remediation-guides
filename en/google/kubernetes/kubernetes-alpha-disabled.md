[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Kubernetes Alpha Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Kubernetes Alpha Disabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensure the GKE Cluster alpha cluster feature is disabled. |
| **More Info** | It is recommended to not use Alpha clusters as they expire after thirty days and do not receive security updates. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/concepts/alpha-clusters |
| **Recommended Action** | 1. Create a new cluster with the alpha feature disabled. 2. Migrate all required cluster data from the cluster with alpha to this newly created cluster. 3.Delete the engine cluster with alpha enabled. |

## Detailed Remediation Steps
