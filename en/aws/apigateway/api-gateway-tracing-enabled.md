[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Tracing Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Tracing Enabled |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway API stages have tracing enabled for AWS X-Ray. |
| **More Info** | API Gateway API stages should have tracing enabled to send traces to AWS X-Ray for enhanced distributed tracing. |
| **AWS Link** | https://docs.aws.amazon.com/xray/latest/devguide/xray-services-apigateway.html |
| **Recommended Action** | Enable tracing on API Gateway API stages |

## Detailed Remediation Steps
Enable active tracing on your API stages to sample incoming requests and send traces to X-Ray. </br>
1. Open the API Gateway console at https://console.aws.amazon.com/apigateway/. </br>
2. Choose an API. </br>
3. Choose a stage. </br>
4. On the Logs/Tracing tab, choose Enable X-Ray Tracing and then choose Save Changes. </br>
5. Choose Resources in the left side navigation panel. </br>
6. To redeploy the API with the new settings, choose the Actions dropdown, and then choose Deploy API. </br>
Note: API Gateway uses sampling rules that you define in the X-Ray console to determine which requests to record. </br>
For more info see: https://docs.aws.amazon.com/xray/latest/devguide/xray-console-sampling.html </br>