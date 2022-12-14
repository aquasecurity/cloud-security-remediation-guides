[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPC Endpoint Cross Account Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Endpoint Cross Account Access |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that Amazon VPC endpoints do not allow unknown cross account access. |
| **More Info** | VPC endpoints should not allow unknown cross account access to avoid any unsigned requests made to the services inside VPC. |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/vpc-endpoints-access.html |
| **Recommended Action** | Update VPC endpoint access policy in order to remove untrusted cross account access |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for VPC. </br> 
3. To update a VPC endpoint policy, in the navigation pane, choose Endpoints. </br>
4. Select the VPC endpoint. </br>
5. Choose Actions, Manage policy. </br>
6. Update the policy to not allow unknown cross account access. </br>
7. Choose Save. </br>