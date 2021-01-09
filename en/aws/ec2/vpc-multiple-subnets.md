[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPC Multiple Subnets

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Multiple Subnets |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that VPCs have multiple subnets to provide a layered architecture |
| **More Info** | VPCs should be designed to have separate public and private subnets, ideally across availability zones, enabling a DMZ-style architecture. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Subnets.html#SubnetSecurity |
| **Recommended Action** | Create at least two subnets in each VPC, utilizing one for public traffic and the other for private traffic. |

## Detailed Remediation Steps

