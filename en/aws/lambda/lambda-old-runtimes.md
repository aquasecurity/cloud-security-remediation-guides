[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Lambda / Lambda Old Runtimes

## Quick Info

| | |
|-|-|
| **Plugin Title** | Lambda Old Runtimes |
| **Cloud** | AWS |
| **Category** | Lambda |
| **Description** | Ensures Lambda functions are not using out-of-date runtime environments. |
| **More Info** | Lambda runtimes should be kept current with recent versions of the underlying codebase. Deprecated runtimes should not be used. |
| **AWS Link** | http://docs.aws.amazon.com/lambda/latest/dg/current-supported-versions.html |
| **Recommended Action** | Upgrade the Lambda function runtime to use a more current version. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Lambda. </br> <img src="/resources/aws/lambda/lambda-old-runtimes/step2.png"/>
3. Scroll down the left navigation panel and choose "Functions".</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step3.png"/>
4. Select the Lambda function that needs to be verify from "Functions name".</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step4.png"/>
5. On the "Lambda Functions" page scroll down and choose "Configuration".</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step5.png"/>
6. Scroll down the "Configuration" tab and check the "Runtime" value and verify the "Runtime" environment using the latest version of the software or not.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step6.png"/>
7. Repeat step number 2 - 6 to verify other "Lambda functions" in the selected region.</br>
8. Navigate to "AWS Lambda" and choose "Lambda function" that needs to modify to use the latest version of the software supported by AWS.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step8.png"/>
9. Choose the "Configuration" tab and scroll down and open the "Runtime" environment dropdown menu.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step9.png"/>
10. Select the latest version from the "Runtime" environment for the selected "Lambda fucntion" and click on the "Save" button at the top of the dashboard.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step10.png"/>
11. Repeat steps number 8 - 10 to modify "Runtime" environment for other "Lambda functions" in the selected region.</br>
