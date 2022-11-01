[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPC Subnet Instances Present

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Subnet Instances Present |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that there are instances attached to every subnet |
| **More Info** | All subnets should have instances associated and unused subnets should be removed to avoid reaching the limit |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints-access.html |
| **Recommended Action** | UUpdate VPC subnets and attach instances to it or remove the unused VPC subnets |

## Detailed Remediation Steps
To update a VPC endpoint policy </br>
1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Endpoints. </br>
3. Select the VPC endpoint. </br>
4. Choose Actions, Manage policy. </br>
5. Choose Full Access to allow full access to the service, or choose Custom and attach a custom policy. </br>
6. Choose Save. </br>