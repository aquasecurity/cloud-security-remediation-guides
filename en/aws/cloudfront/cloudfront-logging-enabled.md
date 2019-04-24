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
4. Click the "Distribution Settings" button from Menu to get into the "CloudFront Distribution" configuration page. </br>
5. Click the "Edit" button from the  "General" tab on the top menu. </br>
6. In the "Distribution Settings" tab scroll down and verify the "Logging" feature configuration status. If Logging is "Off" then it cannot create log files that contain detailed information about every user request that CloudFront receives.</br>
7. 
