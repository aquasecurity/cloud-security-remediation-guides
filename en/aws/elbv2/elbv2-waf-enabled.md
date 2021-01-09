[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 WAF Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 WAF Enabled |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensure that all Application Load Balancers have WAF enabled. |
| **More Info** | Enabling WAF allows control over requests to the load balancer, allowing or denying traffic based off rules in the Web ACL |
| **AWS Link** | https://aws.amazon.com/blogs/aws/aws-web-application-firewall-waf-for-application-load-balancers/ |
| **Recommended Action** | 1. Enter the WAF service. 2. Enter Web ACLs and filter by the region the Application Load Balancer is in. 3. If no Web ACL is found, Create a new Web ACL in the region the ALB resides and in Resource type to associate with web ACL, select the Load Balancer.  |

## Detailed Remediation Steps




