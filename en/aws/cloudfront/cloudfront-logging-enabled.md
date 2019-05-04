[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / CloudFront Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Logging Enabled |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensures CloudFront distributions have request logging enabled. |
| **More Info** | Logging requests to CloudFront distributions is a helpful way of detecting and investigating potential attacks, malicious activity, or misuse of backend resources. Logs can be sent to S3 and processed for further analysis. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/AccessLogs.html |
| **Recommended Action** | Enable CloudFront request logging. |

## Detailed Remediation Steps
1. Log into to the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step2.png"/>
3. Select the "CloudFront Distribution" that needs to be verified.</br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step3.png"/>
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br><img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step4.png"/>
5. Click the "Edit" button from the  "General" tab on the top menu. </br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step5.png"/>
6. In the "Distribution Settings" tab scroll down and verify the "Logging" feature configuration status. If Logging is "Off" then it cannot create log files that contain detailed information about every user request that CloudFront receives.</br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step6.png"/>
7. Click on the "ON" option to initiate the Logging feature of CloudFront to log all viewer requests for files in your distribution.</br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step7.png"/>
8. Click on "Bucket for Logs" feature and specify the Amazon S3 bucket in which you want CloudFront to save web access logs.</br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step8.png"/>
9. Click on Log Prefix which is optional for the names of log files.</br> <img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step9.png"/>
10. Scroll down and click on "Yes,Edit" to save the changes.</br><img src="/resources/aws/cloudfront/cloudfront-logging-enabled/step10.png"/>
11. Repeat the steps number 5 and 6 to establish any other "CloudFront Distribution" has Logging enabled or not.
