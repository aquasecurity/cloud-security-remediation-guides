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
5. Click the "Edit" button from the  General tab on the top menu. </br>![Step 5](/resources/aws/cloudfront/secure-cloudfront-origin/step5.png "Step 5 - Edit")
6. Scroll down and choose the "Security Policy" that you want CloudFront to use for HTTPS connections and must use TLSv1.1 or higher SSL protocols.</br>![Step 6](/resources/aws/cloudfront/secure-cloudfront-origin/step6.png "Step 6 - Security Policy")
7. Scroll down and click on "Yes,Edit" to save the changes.</br>![Step 7](/resources/aws/cloudfront/secure-cloudfront-origin/step7.png "Step 7 - Edit")
8. Click the "Behaviors" button from the top menu to get into the "Behaviors" configuration page and select the "Behavior" which needs to be verified.</br>![Step 8](/resources/aws/cloudfront/secure-cloudfront-origin/step8.png "Step 8 - Behaviors")
9. On the Default Cache Behavior Settings, verify the "Viewer Protocol Policy" and if "HTTP and HTTPS" is selected than CloudFront allows viewers to access your web content using either HTTP or HTTPS.</br>![Step 9](/resources/aws/cloudfront/secure-cloudfront-origin/step9.png "Step 9 - Viewer Protocol Policy")
10.  On the "Viewer Protocol Policy" choose "HTTPS Only" so CloudFront allows viewers to access your content only if they're using HTTPS.</br>![Step 10](/resources/aws/cloudfront/secure-cloudfront-origin/step10.png "Step 10 - HTTPS")
11. Scroll down and click on "Yes,Edit" to save the changes.</br>![Step 11](/resources/aws/cloudfront/secure-cloudfront-origin/step11.png "Step 11 - Edit")
12. CloudFront Distribution has traffic sent between CloudFront and its origin over HTTPS and uses TLSv1.1 or higher now. </br>
