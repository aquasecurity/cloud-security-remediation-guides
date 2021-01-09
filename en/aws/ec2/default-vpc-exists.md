[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Default VPC Exists

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default VPC Exists |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determines whether the default VPC exists. |
| **More Info** | The default VPC should not be used in order to avoid launching multiple services in the same network which may not require connectivity. Each application, or network tier, should use its own VPC. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/default-vpc.html |
| **Recommended Action** | Move resources from the default VPC to a new VPC created for that application or resource group. |

## Detailed Remediation Steps




