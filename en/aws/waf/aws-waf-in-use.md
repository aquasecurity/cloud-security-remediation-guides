[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / WAF / AWS WAF In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | AWS WAF In Use |
| **Cloud** | AWS |
| **Category** | WAF |
| **Description** | Ensure that AWS Web Application Firewall (WAF) is in use to achieve availability and security for AWS-powered web applications |
| **More Info** | Using WAF for your web application running in AWS environment can help against common web-based attacks, SQL injection attacks, DDOS attacks and more |
| **AWS Link** | https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html |
| **Recommended Action** | Create one or more WAF ACLs with proper actions and rules |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console and open the AWS WAF console at https://console.aws.amazon.com/wafv2/. </br>
2. From the AWS WAF home page, choose Create web ACL. </br>
3. For Name, enter the name that you want to use to identify this web ACL. </br>
4. For Description - (optional), enter a longer description for the web ACL. </br>
5. For CloudWatch metric name, change the default name if applicable. Follow the guidance on the console for valid characters. The name can't contain special characters, white space, or metric names reserved for AWS WAF, including "All" and "Default_Action." </br>
6. Choose the AWS resources that you want AWS WAF to inspect web requests for. these steps covers the steps for Amazon CloudFront. The process is essentially the same for an Amazon API Gateway REST API, an Application Load Balancer, an AWS AppSync GraphQL API, or an Amazon Cognito user pool. </br>
7. Choose CloudFront distributions. The Region automatically populates to Global (CloudFront) for CloudFront distributions. </br>
8. (Optional) For Associated AWS resources, choose Add AWS resources. In the dialog box, choose the resources that you want to associate, and then choose Add. AWS WAF returns you to the Describe web ACL and associated AWS resources page. </br>
9. Choose Next. </br>
10. Add the rules and rule groups that you want to use to filter web requests. For example, you can specify the IP addresses that the requests originate from and values in the request that are used only by attackers. For each rule, you specify how to handle matching web requests. You can block them, allow them, count them, or insert a CAPTCHA check against them. You define an action for each rule that you define inside a web ACL and for each rule that you define inside a rule group. </br>
11. Specify a default action for the web ACL, either Block or Allow. This is the action that AWS WAF takes when a web request doesn't match any of the rules. </br>
12. Review then click on Create web ACL. </br>
13. To Associate a web ACL with an AWS resource, see this link: https://docs.aws.amazon.com/waf/latest/developerguide/web-acl-associating-aws-resource.html </br>