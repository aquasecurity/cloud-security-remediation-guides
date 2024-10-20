
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Kubernetes Service / Kubernetes Service Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Azure Kubernetes Service Has Tags |
| **Cloud** | AZURE |
| **Category** | Containers |
| **Description** | Ensures the Azure Kubernetes Service Has Tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/aks/use-tags |
| **Recommended Action** | Modify Kubernetes service and add tags |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Kubernetes Service". </br> <img src="/resources/azure/kubernetesservice/aks-has-tags/step2.png"/>
3. On the "Kubernetes Service" page, select the cluster that needs to have tags. </br> <img src="/resources/azure/kubernetesservice/aks-has-tags/step3.png"/>
4. On the Cluster details page Slect "Tags" from the left navigation panel.</br> <img src="/resources/azure/kubernetesservice/aks-has-tags/step4.png"/>
5. On "Tags" page enter the name/value of the tag you want to add and click "Apply" on the bottom of the page" </br> <img src="/resources/azure/kubernetesservice/aks-has-tags/step5.png"/>
