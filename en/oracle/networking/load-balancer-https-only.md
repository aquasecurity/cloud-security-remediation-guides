[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Load Balancer HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | Load Balancer HTTPS Only |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Ensures LBs are configured to only accept connections on HTTPS ports. |
| **More Info** | For maximum security, LBs can be configured to only accept HTTPS connections. Standard HTTP connections  will be blocked. This should only be done if the  client application is configured to query HTTPS  directly and not rely on a redirect from HTTP. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Balance/Tasks/managinglisteners.htm |
| **Recommended Action** | Remove non-HTTPS listeners from load balancer. |

## Detailed Remediation Steps

