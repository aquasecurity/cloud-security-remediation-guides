[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / CLB / CLB HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | CLB HTTPS Only |
| **Cloud** | GOOGLE |
| **Category** | CLB |
| **Description** | Ensures CLBs are configured to only accept connections on HTTPS ports |
| **More Info** | For maximum security, CLBs can be configured to only accept HTTPS connections. Standard HTTP connections will be blocked. This should only be done if the client application is configured to query HTTPS directly and not rely on a redirect from HTTP. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/vpc |
| **Recommended Action** | Remove non-HTTPS listeners from the load balancer. |

## Detailed Remediation Steps


