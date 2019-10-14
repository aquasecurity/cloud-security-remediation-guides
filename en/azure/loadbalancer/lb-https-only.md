[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Load Balancer / LB HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | LB HTTPS Only |
| **Cloud** | AZURE |
| **Category** | Load Balancer |
| **Description** | Ensures load balancers are configured to only accept connections on HTTPS ports |
| **More Info** | For maximum security, load balancers can be configured to only accept HTTPS connections. Standard HTTP connections will be blocked. This should only be done if the client application is configured to query HTTPS directly and not rely on a redirect from HTTP. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-overview |
| **Recommended Action** | Ensure that each load balancer only accepts connections on port 443. |

## Detailed Remediation Steps

