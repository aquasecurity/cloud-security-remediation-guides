[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 HTTPS Only |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensures ELBs are configured to only accept connections on HTTPS ports. |
| **More Info** | For maximum security, ELBs can be configured to only accept HTTPS connections. Standard HTTP connections  will be blocked. This should only be done if the  client application is configured to query HTTPS  directly and not rely on a redirect from HTTP. |
| **AWS Link** | http://docs.aws.amazon.com/ElasticLoadBalancing/latest/DeveloperGuide/elb-security-policy-options.html |
| **Recommended Action** | Remove non-HTTPS listeners from load balancer. |

## Detailed Remediation Steps




