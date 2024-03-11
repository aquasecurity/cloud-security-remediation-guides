[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway WAF Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway WAF Enabled |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that API Gateway APIs are associated with a Web Application Firewall. |
| **More Info** | API Gateway APIs should be associated with a Web Application Firewall to ensure API security. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-control-access-aws-waf.html |
| **Recommended Action** | Associate API Gateway API with Web Application Firewall |

## Detailed Remediation Steps
To associate an AWS WAF regional Web ACL with an API Gateway API stage using the API Gateway console </br>
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. In the APIs navigation pane, choose the API, and then choose Stages. </br>
3. In the Stages pane, choose the name of the stage. </br>
4. In the Stage Editor pane, choose the Settings tab. </br>
5. To associate a Regional web ACL with the API stage: </br>
a. In the AWS WAF web ACL dropdown list, choose the Regional web ACL that you want to associate with this stage.
Note: </br>
If the web ACL you need doesn't exist yet, choose Create WebACL. Then choose Go to AWS WAF to open the AWS WAF console in a new browser tab and create a Regional web ACL. Then return to the API Gateway console to associate the web ACL with the stage. </br>
6. Choose Save Changes. </br>