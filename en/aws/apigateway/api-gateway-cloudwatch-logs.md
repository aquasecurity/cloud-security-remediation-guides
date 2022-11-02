[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway CloudWatch Logs

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway CloudWatch Logs |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway API stages have Amazon CloudWatch Logs enabled |
| **More Info** | API Gateway API stages should have Amazon CloudWatch Logs enabled to help debug issues related to request execution or client access to your API. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/set-up-logging.html |
| **Recommended Action** | Modify API Gateway API stages to enable CloudWatch Logs |

## Detailed Remediation Steps
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. Choose a REST API. </br>
3. Choose Settings from the primary navigation panel and enter an ARN of an IAM role with appropriate permissions in CloudWatch log role ARN. You need to do this once. </br>
4. Choose an existing API and then choose a stage. </br>
5. Choose Logs/Tracing in the Stage Editor. </br>
6. To enable execution logging: </br>
a. Choose Enable CloudWatch Logs under CloudWatch Settings. </br>
b. Choose Error or Info from the dropdown menu. </br>
c. If desired, choose Log full requests/responses data to log the full API requests and responses. </br>
Warning: This can be useful to troubleshoot APIs, but can result in logging sensitive data. We recommend that you don't enable Log full requests/responses data for production APIs. </br>
d. If desired, choose Enable Detailed CloudWatch Metrics. </br>
7. To enable access logging: </br>
a. Choose Enable Access Logging under Custom Access Logging. </br>
b. Enter the ARN of a log group in Access Log Destination ARN. The ARN format is arn:aws:logs:{region}:{account-id}:log-group:log-group-name. </br>
c. Enter a log format in Log Format. You can choose CLF, JSON, XML, or CSV to use one of the provided examples as a guide. </br>
8. Choose Save Changes. </br>