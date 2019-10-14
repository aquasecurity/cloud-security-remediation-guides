[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Load Balancer / LB No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | LB No Instances |
| **Cloud** | AZURE |
| **Category** | Load Balancer |
| **Description** | Detects load balancers that have no backend instances attached |
| **More Info** | All load balancers should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old load balancers with no instances pose a security concern if new instances are accidentally attached. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-overview |
| **Recommended Action** | Delete old load balancers that no longer have backend resources. |

## Detailed Remediation Steps

