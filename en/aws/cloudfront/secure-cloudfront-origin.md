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
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/secure-cloudfront-origin/step2.png"/>
3. Select the "CloudFront Distribution" that needs to be verified.</br> <img src="/resources/aws/cloudfront/secure-cloudfront-origin/step3.png"/>
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br><img src="/resources/aws/cloudfront/secure-cloudfront-origin/step4.png"/>
5. Select the Origins tab and choose the distribution origin that needs to be verified.</br><img src="/resources/aws/cloudfront/secure-cloudfront-origin/step5.png"/>
6. On the Origin Settings page, ensure TLSv1.1 or higher protocol is enabled.</br> <img src="/resources/aws/cloudfront/secure-cloudfront-origin/step6.png"/>
7. On the Origin Settings page, verify the "Origin Protocol Policy" is set to "HTTPS Only".<img src="/resources/aws/cloudfront/secure-cloudfront-origin/step7.png"/>
8. Scroll down and click on "Yes,Edit" and save the changes.</br><img src="/resources/aws/cloudfront/secure-cloudfront-origin/step8.png"/>
9. Repeat steps number 5, 6 and 7 to verify another CloudFront Distribution.</br>
