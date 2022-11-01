[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Latest Platform Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Latest Platform Version |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensure that EKS clusters are using latest platform version |
| **More Info** | Amazon EKS platform versions represent the capabilities of the Amazon EKS cluster control plane, such as which Kubernetes API server flags are enabled, as well as the current Kubernetes patch version. Clusters should be kept up to date of latest platforms to ensure Kubernetes security patches are applied. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/platform-versions.html |
| **Recommended Action** | Check for the version on all EKS clusters to be the latest platform version. |

## Detailed Remediation Steps
1. Amazon EKS automatically upgrades all existing clusters to the latest Amazon EKS platform version. </br>
2. If your cluster is more than two platform versions behind the current platform version, then it's possible that Amazon EKS wasn't able to automatically update your cluster. </br>
3. Check this link to troubleshoot the issue: https://docs.aws.amazon.com/eks/latest/userguide/troubleshooting.html#troubleshooting-platform-version </br>