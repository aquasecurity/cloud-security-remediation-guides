[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / IP Forwarding Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | IP Forwarding Disabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that IP forwarding is disabled on all instances |
| **More Info** | Disabling IP forwarding ensures that the instance only sends and receives packets with matching destination or source IPs. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-routes |
| **Recommended Action** | IP forwarding settings can only be chosen when creating a new instance. Delete the affected instances and redeploy with IP forwarding disabled. |

## Detailed Remediation Steps


