[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Excessive Security Lists

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Security Lists |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Determine if there are an excessive number of security lists in the account |
| **More Info** | Keeping the number of security lists to a minimum helps reduce the attack surface of an account. Rather than creating new groups with the same rules for each project, common rules should be grouped under the same security lists. For example, instead of adding port 22 from a known IP to every group, create a single "SSH" security group which can be used on multiple instances. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Network/Concepts/securitylists.htm |
| **Recommended Action** | Limit the number of security lists to prevent accidental authorizations |

## Detailed Remediation Steps

