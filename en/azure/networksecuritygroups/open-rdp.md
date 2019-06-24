[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open RDP

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open RDP |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP port 3389 for RDP is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as RDP should be restricted to known IP addresses. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | For each VM, open the Networking blade and verify that the Inbound Port Rules do not have a rule for RDP with a source equal to "Any" OR "Internet" |

## Detailed Remediation Steps

