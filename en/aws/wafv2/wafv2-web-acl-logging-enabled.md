[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / WAF / Web ACL Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Web ACL Logging Enabled |
| **Cloud** | AWS |
| **Category** | WAF |
| **Description** | Ensure that AWS WAFV2 Web Access Control Lists (ACLs) have logging enabled. |
| **More Info** | Enabling logging for Web ACL allows detailed logging of web requests that match defined rules within the WAF Web ACL. This enables comprehensive monitoring, analysis, and troubleshooting of security threats and traffic patterns within your web application. |
| **AWS Link** | https://docs.aws.amazon.com/waf/latest/developerguide/logging-management.html |
| **Recommended Action** | Modify WAFV2 Web ACL and enable logging. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "WAF & Shield".</br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step2.png"/>
3. On "WAF & Shield Dashboard" page, Click on "Web ACLs" from left navigation panel.</br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step3.png"/>
4. On WAF Web ACLs list page, Click on the Web ACLs name on which you want to enable logging.</br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step4.png"/>
5. On Web ACLs details page scroll down and choose "Logging and metrics" option.</br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step5.png"/>
6. Scroll down, and under the "Logging" section click on "Enable" button.</br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step6.png"/>
7. On "Enable Logging" page select the Logging Destination for Logs. </br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step7.png"/> 
8. Scroll to bottom of Page and click "Save" button. </br> <img src="/resources/aws/wafv2/wafv2-web-acl-logging-enabled/step8.png"/> 
