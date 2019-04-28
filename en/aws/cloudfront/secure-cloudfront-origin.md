[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / Secure CloudFront Origin

## Quick Info

| | |
|-|-|
| **Plugin Title** | Secure CloudFront Origin |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Detects the use of secure web origins with secure protocols for CloudFront. |
| **More Info** | Traffic passed between the CloudFront edge nodes and the backend resource should be sent over HTTPS with modern protocols for all web-based origins. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/distribution-web.html |
| **Recommended Action** | Ensure that traffic sent between CloudFront and its origin is passed over HTTPS and uses TLSv1.1 or higher. Do not use the match-viewer option. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront/secure-cloudfront-origin/step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that needs to be verified.</br> ![Step 3](/resources/aws/cloudfront/secure-cloudfront-origin/step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront/secure-cloudfront-origin/step4.png "Step 4 - Distribution Settings")
5. Select the Origins tab and choose the distribution origin that needs to be verified.</br>![Step 5](/resources/aws/cloudfront/secure-cloudfront-origin/step5.png "Step 5 - Origins")
6. On the Origin Settings page, ensure TLSv1.1 or higher protocol is enabled.</br>![Step 6](/resources/aws/cloudfront/secure-cloudfront-origin/step6.png "Step 6 - Origin Settings")
7. On the Origin Settings page, verify the "Origin Protocol Policy" is set to "HTTPS Only".![Step 7](/resources/aws/cloudfront/secure-cloudfront-origin/step7.png "Step 7 - Protocol Policy")
8. Scroll down and click on "Yes,Edit" and save the changes.![Step 8](/resources/aws/cloudfront/secure-cloudfront-origin/step8.png "Step 8 - Edit")
9. Repeat steps number 5, 6 and 7 to verify another CloudFront Distribution.</br>
