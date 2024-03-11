[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Secrets Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Secrets Encrypted |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensures EKS clusters are configured to enable envelope encryption of Kubernetes secrets using KMS |
| **More Info** | Amazon EKS clusters should be configured to enable envelope encryption for Kubernetes secrets to adhere to security best practice for applications that store sensitive data. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2020/03/amazon-eks-adds-envelope-encryption-for-secrets-with-aws-kms/ |
| **Recommended Action** | Modify EKS clusters to enable envelope encryption for Kubernetes secrets |

## Detailed Remediation Steps
1. Open the Amazon EKS console at https://console.aws.amazon.com/eks/home#/clusters </br>
2. Choose the name of the cluster to display your cluster information. </br>
3. Choose the Preview tab and under section Secrets encryption Click Enable. </br>
4. Select KMS Key and click enable. </br>
5. It will as you to confirm because once encryption enabled it can't be removed or undone. </br>
6. Click Confirm. </br>