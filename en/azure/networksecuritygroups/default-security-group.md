[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Default Security Group

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default Security Group |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Ensure the default security groups block all traffic by default. |
| **More Info** | The default security group is often used for resources launched without a defined security group. For this reason, the default rules should be to block all traffic to prevent an accidental exposure. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Update the rules for the default security group to deny all traffic by default. |

## Detailed Remediation Steps

