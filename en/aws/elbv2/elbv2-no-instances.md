[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 No Instances |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Detects ELBs that have no target groups attached |
| **More Info** | All ELBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old ELBs with no target groups present a security concern if new target groups are accidentally attached. |
| **AWS Link** | https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html |
| **Recommended Action** | Delete old ELBs that no longer have backend resources. |

## Detailed Remediation Steps




