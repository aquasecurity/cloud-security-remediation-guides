[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open Salt

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Salt |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP ports 4505 or 4506 for the Salt master are open to the public |
| **More Info** | Active Salt vulnerabilities, CVE-2020-11651 and CVE-2020-11652 are exploiting Salt instances exposed to the internet. These ports should be closed immediately. |
| **AZURE Link** | https://help.saltstack.com/hc/en-us/articles/360043056331-New-SaltStack-Release-Critical-Vulnerability |
| **Recommended Action** | Restrict TCP ports 4505 and 4506 to known IP addresses |

## Detailed Remediation Steps

