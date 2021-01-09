[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / CloudFront WAF Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront WAF Enabled |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensures CloudFront distributions have WAF enabled. |
| **More Info** | Enabling WAF allows control over requests to the Cloudfront Distribution, allowing or denying traffic based off rules in the Web ACL |
| **AWS Link** | https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-associating-cloudfront-distribution.html |
| **Recommended Action** | 1. Enter the WAF service. 2. Enter Web ACLs and filter by global. 3. If no Web ACL is found, Create a new global Web ACL and in Resource type to associate with web ACL, select the Cloudfront Distribution.  |

## Detailed Remediation Steps




