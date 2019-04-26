[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / CloudFront HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront HTTPS Only |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensures CloudFront distributions are configured to redirect non-HTTPS traffic to HTTPS. |
| **More Info** | For maximum security, CloudFront distributions can be configured to only accept HTTPS connections or to redirect HTTP connections to HTTPS. |
| **AWS Link** | http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/CloudFront.html |
| **Recommended Action** | Remove HTTP-only listeners from distributions. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront//step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that needs to be verified.</br> ![Step 3](/resources/aws/cloudfront/cloudfront-/step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront/cloudfront-/step4.png "Step 4 - Distribution Settings")
5. Click the "Behaviors" button from top menu to get into the "Behaviors" configuration page. </br> ![Step 5](/resources/aws/cloudfront/cloudfront-/step5.png "Step 5 - Behaviors ")
6. 
