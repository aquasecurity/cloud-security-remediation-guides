[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Excessive Firewall Rules

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Firewall Rules |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Determines if there are an excessive number of firewall rules in the account |
| **More Info** | Keeping the number of firewall rules to a minimum helps reduce the attack surface of an account. Rather than creating new rules with the same rules for each project, common rules should be grouped under the same firewall rule. For example, instead of adding port 22 from a known IP to every firewall rule, create a single "SSH" firewall rule which can be used on multiple instances. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-firewalls |
| **Recommended Action** | Limit the number of firewall rules to prevent accidental authorizations |

## Detailed Remediation Steps


