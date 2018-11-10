[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELB No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELB No Instances |
| **Cloud** | AWS |
| **Category** | ELB |
| **Description** | Detects ELBs that have no backend instances attached |
| **More Info** | All ELBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old ELBs with no instances present a security concern if new instances are accidentally attached. |
| **AWS Link** | http://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-backend-instances.html |
| **Recommended Action** | Delete old ELBs that no longer have backend resources. |

## Detailed Remediation Steps

