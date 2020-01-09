[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Level SSH Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Level SSH Only |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that instances are not configured to allow project-wide SSH keys |
| **More Info** | To support the principle of least privilege and prevent potential privilege escalation it is recommended that instances are not give access to project-wide SSH keys through instance metadata. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys |
| **Recommended Action** | Ensure project-wide SSH keys are blocked for all instances. |

## Detailed Remediation Steps


