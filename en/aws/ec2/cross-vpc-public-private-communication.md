[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Cross VPC Public Private Communication

## Quick Info

| | |
|-|-|
| **Plugin Title** | Cross VPC Public Private Communication |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures communication between public and private VPC tiers is not enabled |
| **More Info** | Communication between the public tier of one VPC and the private tier of other VPCs should never be allowed. Instead, VPC peerings with proper NACLs and gateways should be used |
| **AWS Link** | https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Subnets.html |
| **Recommended Action** | Remove the NACL rules allowing communication between the public and private tiers of different VPCs |

## Detailed Remediation Steps

