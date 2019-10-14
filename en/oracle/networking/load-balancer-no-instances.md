[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Load Balancer No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | Load Balancer No Instances |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Detects LBs that have no backend instances attached |
| **More Info** | All LBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old ELBs with no instances present a security concern if new instances are accidentally attached. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/GSG/Tasks/loadbalancing.htm |
| **Recommended Action** | Delete old LBs that no longer have backend resources. |

## Detailed Remediation Steps

