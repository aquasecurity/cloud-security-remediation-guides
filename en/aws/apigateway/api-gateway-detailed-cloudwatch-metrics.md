[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Detailed CloudWatch Metrics

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Detailed CloudWatch Metrics |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that API Gateway API stages have detailed CloudWatch metrics enabled. |
| **More Info** | API Gateway API stages should have detailed CloudWatch metrics enabled to monitor logs and events. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-metrics.html |
| **Recommended Action** | Add CloudWatch role ARN to API settings and enabled detailed metrics for each stage |

## Detailed Remediation Steps
1. Open the API Gateway console at https://console.aws.amazon.com/apigateway/. </br>
2. Choose an API. </br>
3. Choose a stage. </br>
4. On the Logs/Tracing tab, choose Enable Detailed CloudWatch Metrics. </br>
5. Choose Resources in the left side navigation panel. </br>
6. To redeploy the API with the new settings, choose the Actions dropdown, and then choose Deploy API. </br>