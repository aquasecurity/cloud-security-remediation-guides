[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Instances Least Privilege

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instances Least Privilege |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that instances are not configured to use the default service account with full access to all cloud APIs |
| **More Info** | To support the principle of least privilege and prevent potential privilege escalation, it is recommended that instances are not assigned to the default service account, Compute Engine default service account with a scope allowing full access to all cloud APIs. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances |
| **Recommended Action** | For all instances, if the default service account is used, ensure full access to all cloud APIs is not configured. |

## Detailed Remediation Steps


