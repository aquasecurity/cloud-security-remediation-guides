[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Security Groups |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensures the EKS control plane only allows inbound traffic on port 443. |
| **More Info** | The EKS control plane only requires port 443 access. Security groups for the control plane should not add additional port access. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/sec-group-reqs.html |
| **Recommended Action** | Configure security groups for the EKS control plane to allow access only on port 443. |

## Detailed Remediation Steps




