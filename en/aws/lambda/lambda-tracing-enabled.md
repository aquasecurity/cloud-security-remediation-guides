[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Lambda / Lambda Tracing Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Lambda Tracing Enabled |
| **Cloud** | AWS |
| **Category** | Lambda |
| **Description** | Ensures AWS Lambda functions have active tracing for X-Ray. |
| **More Info** | AWS Lambda functions should have active tracing in order to gain visibility into the functions execution and performance. |
| **AWS Link** | https://docs.aws.amazon.com/lambda/latest/dg/services-xray.html |
| **Recommended Action** | Modify Lambda functions to activate tracing. |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for Lambda. </br> 
3. Scroll down the left navigation panel and choose "Functions".</br> 
4. Select the Lambda function that needs to be verify from "Functions name".</br> 
5. On the "Lambda Functions" page scroll down and choose "Configuration".</br>
6. Scroll down the "Configuration" tab and choose the "Monitoring and operations tools". </br>
7. Under X-Ray, toggle on Active tracing. </br>
8. Click on the "Save" button at the top of the dashboard.</br>
9. Repeat steps 4 - 8 to enable active tracing for other "Lambda functions" in the selected region.</br>