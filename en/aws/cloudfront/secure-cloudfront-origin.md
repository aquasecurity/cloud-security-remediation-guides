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
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront//step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that needs to be verified.</br> ![Step 3](/resources/aws/cloudfront//step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront//step4.png "Step 4 - Distribution Settings")
5. Click the "Edit" button from the  General tab on the top menu. </br>![Step 5](/resources/aws/cloudfront//step5.png "Step 5 - Edit")
6. Scroll down and choose the "Security Policy" that you want CloudFront to use for HTTPS connections and must use TLSv1.1 or higher SSL protocols.</br>![Step 6](/resources/aws/cloudfront//step6.png "Step 6 - Security Policy")
7. Scroll down and click on "Yes,Edit" to save the changes.
8. Click the "Behaviors" button from the top menu to get into the "Behaviors" configuration page and select the "Behavior" which needs to be verified.</br>
9. On the Default Cache Behavior Settings, verify the "Viewer Protocol Policy" and if "HTTP and HTTPS" is selected than CloudFront allows viewers to access your web content using either HTTP or HTTPS.</br>
10.  On the "Viewer Protocol Policy" choose "HTTPS Only" so CloudFront allows viewers to access your content only if they're using HTTPS.</br>
11. Scroll down and click on "Yes,Edit" to save the changes.</br>
12. CloudFront Distribution has traffic sent between CloudFront and its origin over HTTPS and uses TLSv1.1 or higher now. </br>
