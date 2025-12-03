[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Cross Organization VPC Peering Connections

## Quick Info

| | |
|-|-|
| **Plugin Title** | Cross Organization VPC Peering Connections |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that VPC peering communication is only between AWS accounts, members of the same AWS Organization |
| **More Info** | VPC peering communication should be only between AWS accounts to keep organization resources private and isolated |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/peering/working-with-vpc-peering.html |
| **Recommended Action** | Update VPC peering connections to allow connections to AWS Accounts, members of the same organization |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for VPC. </br> 
3. In the navigation pane, choose Peering Connections. </br>
4. Select the VPC peering connection that allows communication with accounts outside the AWS organization, and choose Actions, Delete Peering connection. </br>
5. Repeat steps 3-4 for all VPC peering connections that allow connections outside AWS organization. </br>