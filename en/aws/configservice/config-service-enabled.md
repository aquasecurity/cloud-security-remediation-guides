[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ConfigService / Config Service Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Config Service Enabled |
| **Cloud** | AWS |
| **Category** | ConfigService |
| **Description** | Ensures the AWS Config Service is enabled to detect changes to account resources |
| **More Info** | The AWS Config Service tracks changes to a number of resources in an AWS account and is invaluable in determining how account changes affect other resources and in recovery in the event of an account intrusion or accidental configuration change. |
| **AWS Link** | https://aws.amazon.com/config/details/ |
| **Recommended Action** | Enable the AWS Config Service for all regions and resources in an account. Ensure that it is properly recording and delivering logs. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for AWS Config. </br> <img src="/resources/aws/configservice/config-service-enabled/step2.png"/>
3. If the AWS console redirects to "Get Started" page then the Config Service is not enabled in the selected region. </br> <img src="/resources/aws/configservice/config-service-enabled/step3.png"/>
4. Repeat steps number 2 - 3 to verify "Config Service" is enabled or not in the other regions. </br>
5. Navigate on "AWS Config" and click on the "Get Started" button. </br> <img src="/resources/aws/configservice/config-service-enabled/step5.png"/>
6. On the "Settings" page under the "Resource types to record" select both "Record all resources supported in this region" to track configuration changes for all AWS resource and "Include global resources" to include any type of global AWS resource such as "AWS IAM resource".</br> <img src="/resources/aws/configservice/config-service-enabled/step6.png"/>
7. On the "Amazon S3 bucket" option choose either of the options available as "Create a bucket" to create a new bucket, "Choose a bucket from your account" to use an existing S3 bucket, "Choose a bucket from another account" as to use S3 bucket from another AWS account as per the requirement.</br> <img src="/resources/aws/configservice/config-service-enabled/step7.png"/>
8. On the "Amazon SNS topic" choose either of the options available as "Create a topic" to create a new simple notification service topic, "Choose a topic from your account" to choose the existing SNS topic and "Choose a topic from another account" to choose the "SNS Topic" from the another AWS account and in the "Topic Name" field enter an unique name for the "SNS Topic". </br> <img src="/resources/aws/configservice/config-service-enabled/step8.png"/>
9. On the "AWS Config role" choose the "Use an existing AWS Config service-linked role" and click on the "Next" button.</br> <img src="/resources/aws/configservice/config-service-enabled/step9.png"/>
10. On the "AWS Config rules" option scroll down the page and click on the "Select All" option to select all the Config can check the configuration of the resources against rules that are defined or can select either one of them and click on the "Next" button. </br> <img src="/resources/aws/configservice/config-service-enabled/step10.png"/>
11. Review the changes and click on the "Confirm" button to make the necessary changes. </br> <img src="/resources/aws/configservice/config-service-enabled/step11.png"/>
12. Repeat steps number 5 - 11 to enable the AWS Config Service for all regions and resources in an account.
