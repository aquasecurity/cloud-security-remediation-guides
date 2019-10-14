[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Level SSH Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Level SSH Only |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that instances are not configured to allow Project Wide SSH keys. |
| **More Info** | To support principle of least privileges and prevent potential privilege escalation it is recommended that instances are not accessible from project wide SSH keys. These keys are accessible through metadata and can become comprimised. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys |
| **Recommended Action** | 1. Enter the Compute Service. 2. Select the Instance in question. 3. Select Edit at the top of the page. 4. Under SSH Keys ensure that Block Project-Wide SSH Keys is enabled. |

## Detailed Remediation Steps

