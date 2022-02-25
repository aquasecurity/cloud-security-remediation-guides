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
4. Select the Lambda function that needs to be verified from "Functions name".</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step4.png"/>
5. On the "Lambda Functions" page scroll down and choose "Code" tab.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step5.png"/>
6. On the "Code" tab scroll down to check for "Runtime settings".</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step6.png"/>
7. To update the "Runtime settings" click on "Edit". </br> <img src="/resources/aws/lambda/lambda-old-runtimes/step7.png"/>
8. On the "Edit runtime settings" open the "Runtime" dropdown.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step8.png"/>
9. From the "Runtime" dropdown verify that the function is using the latest version of runtime environment.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step9.png"/>
10. If the "Runtime" is not at the latest version then select the latest version from the "Runtime" environment for the selected "Lambda function" and click on the "Save" button at the bottom.</br> <img src="/resources/aws/lambda/lambda-old-runtimes/step10.png"/>
11. Repeat steps number 4 - 10 to modify "Runtime" environment for other "Lambda functions" in the selected region.</br>
