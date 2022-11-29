[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Kubernetes Service / AKS Data Encryption at Rest with CMK

## Quick Info

| | |
|-|-|
| **Plugin Title** | AKS Data Encryption at Rest with CMK |
| **Cloud** | AZURE |
| **Category** | Kubernetes Service |
| **Description** | Ensures that Azure Kubernetes Service data is encrypted with CMK |
| **More Info** | AKS Cluster allows you to encrypt your data using customer-managed keys (CMK) instead of using platform-managed keys, which are enabled by default. Your keys encrypt the backup data must be stored in Azure Key Vault.This provides you with full control over the data and the keys. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/aks/azure-disk-customer-managed-keys |
| **Recommended Action** | When creating a new Kubernetes Cluster, ensure that encryption at rest using CMK is enabled under the Node pool tab during creation. |

## Detailed Remediation Steps

