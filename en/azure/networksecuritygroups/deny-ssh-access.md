[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Deny SSH Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Deny SSH Access |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Ensures that all Network Security Group Security Rules deny public SSH access |
| **More Info** | Inbound security group rules should prohibit inbound SSH access from the global address. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-restrict-access-through-internet-facing-endpoints |
| **Recommended Action** | For each Network Security Group attached to a Virtual Machine instance, ensure that the inbound SSH port is appropriately restricted. |

## Detailed Remediation Steps

