[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Default VPC In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default VPC In Use |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Determines whether the default VPC is being used for launching VM instances |
| **More Info** | The default VPC should not be used in order to avoid launching multiple services in the same network which may not require connectivity. Each application, or network tier, should use its own VPC. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/vpc |
| **Recommended Action** | Move resources from the default VPC to a new VPC created for that application or resource group. |

## Detailed Remediation Steps


