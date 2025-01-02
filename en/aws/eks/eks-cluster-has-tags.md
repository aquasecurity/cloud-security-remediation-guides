[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Cluster Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Cluster Has Tags |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensure EKS Cluster have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/eks-using-tags.html |
| **Recommended Action** | Modify EKS Cluster and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "EKS" and Click on "Elastic Kubernetes Services". </br> <img src="/resources/aws/eks/eks-cluster-has-tags/step2.png"/>
3. On "Elastic Kubernetes Services" page Click on Cluster from left navigation panel. </br> <img src="/resources/aws/eks/eks-cluster-has-tags/step3.png"/>
4. On Clusters page Click on the Cluster Name which needs to have tags. </br><img src="/resources/aws/eks/eks-cluster-has-tags/step4.png"/>
5. On Cluster details page choose "Tags" tab from navigation panel on the bottom of page. </br><img src="/resources/aws/eks/eks-cluster-has-tags/step7.png"/>
6. Under the "Tags" tab Click on "Manage Tags" button. </br><img src="/resources/aws/eks/eks-cluster-has-tags/step6.png"/>
7. On manage tags page Click on "Add Tag" button. Enter the key-value for tag and Click "Save Changes" button. </br><img src="/resources/aws/eks/eks-cluster-has-tags/step7.png"/>