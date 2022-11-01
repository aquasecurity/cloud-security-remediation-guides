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
Security groups can be assigned to EKS control plane only during creation. To add additional security groups you have to re-create your cluster. </br>
To add security group to EKS at creation time, follow these steps: </br>
1. Log into the AWS Management Console. </br>
2. Search for EKS. </br>
3. In the navigation pane click on clusters. </br>
4. Click Add Cluster, Ceate. </br>
5. At Step 2: Specify networking, select security group Id, under the Security groupsInfo. </br>
6. If you don't have a security group, create one using VPC console, https://us-west-2.console.aws.amazon.com/vpc/home?#securityGroups </br>
7. For this securoty group allow inbound traffic on port 443 only. </br>
8. Continue the steps to create the cluster. </br>



