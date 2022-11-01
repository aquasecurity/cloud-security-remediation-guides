[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Private Endpoint

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Private Endpoint |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensures the private endpoint setting is enabled for EKS clusters |
| **More Info** | EKS private endpoints can be used to route all traffic between the Kubernetes worker and control plane nodes over a private VPC endpoint rather than across the public internet. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/cluster-endpoint.html |
| **Recommended Action** | Enable the private endpoint setting for all EKS clusters. |

## Detailed Remediation Steps
1. Open the Amazon EKS console at https://console.aws.amazon.com/eks/home#/clusters. </br>
2. Choose the name of the cluster to display your cluster information. </br>
3. Choose the Networking tab and Click Manage Networking. </br>
4. Under Cluster endpoint access select Private. </br>
5. Click Save. </br>



