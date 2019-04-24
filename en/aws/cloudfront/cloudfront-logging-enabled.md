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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront/cloudfront-logging-enabled/step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that need to be verified.</br> ![Step 3](/resources/aws/cloudfront/cloudfront-logging-enabled/step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from Menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront/cloudfront-logging-enabled/step4.png "Step 4 - Distribution Settings")
5. Click the "Edit" button from the  "General" tab on the top menu. </br> ![Step 5](/resources/aws/cloudfront/cloudfront-logging-enabled/step5.png "Step 5 - Edit ")
6. In the "Distribution Settings" tab scroll down and verify the "Logging" feature configuration status. If Logging is "Off" then it cannot create log files that contain detailed information about every user request that CloudFront receives.</br> ![Step 6](/resources/aws/cloudfront/cloudfront-logging-enabled/step6.png "Step 6 - Logging")
7. Click on the "ON" option to initiate the Logging feature of CloudFront to log all viewer requests for files in your distribution.</br> ![Step 7](/resources/aws/cloudfront/cloudfront-logging-enabled/step7.png "Step 7 - ON")
8. Click on "Bucket for Logs" feature and specify the Amazon S3 bucket in which you want CloudFront to save web access logs.</br> ![Step 8](/resources/aws/cloudfront/cloudfront-logging-enabled/step8.png "Step 8 - Bucket for Logs")
9. Click on Log Prefix which is optional for the names of log files.</br> ![Step 9](/resources/aws/cloudfront/cloudfront-logging-enabled/step8.png "Step 9 - Log Prefix")
10. Scroll down and click on "Yes,Edit" to save the changes.</br>![Step 10](/resources/aws/cloudfront/cloudfront-logging-enabled/step8.png "Step 10 - Edit")
11. CloudFront Distribution has CloudFront Logging Enabled now.</br>
