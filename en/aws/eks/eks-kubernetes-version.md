[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Kubernetes Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Kubernetes Version |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensures the latest version of Kubernetes is installed on EKS clusters |
| **More Info** | EKS supports provisioning clusters from several versions of Kubernetes. Clusters should be kept up to date to ensure Kubernetes security patches are applied. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html |
| **Recommended Action** | Upgrade the version of Kubernetes on all EKS clusters to the latest available version. |

## Detailed Remediation Steps

1. Log into the AWS Management Console. </br>
2. Search for EKS. </br>
3. In the navigation pane click on clusters. </br>
4. Click on the cluster you need to check if it has latest EKS Kubernetes version. </br>
5. If there is a new Kubernetes versions available for this cluster, it will show on top with UPDATE NOW button. </br>
6. Click on UPDATE NOW, a pop-up screen will show from which you can choose the Kubernetes version. the default version will be automatically selected. </br>
7. Click Update.


