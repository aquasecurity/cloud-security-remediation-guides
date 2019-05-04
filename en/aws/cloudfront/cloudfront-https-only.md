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
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step2.png"/>
3. Select the "CloudFront Distribution" that needs to be verified.</br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step3.png"/>
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br><img src="/resources/aws/cloudfront/cloudfront-https-only/step4.png"/>
5. Click the "Behaviors" button from the top menu to get into the "Behaviors" configuration page and select the "Behavior" which needs to be verified.</br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step5.png"/>
6. Click the "Edit" button from the "Behaviors" tab on the menu.</br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step6.png"/>
7. On the Default Cache Behavior Settings, verify the "Viewer Protocol Policy" and if "HTTP and HTTPS" is selected than CloudFront allows viewers to access your web content using either HTTP or HTTPS. </br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step7.png"/>
8. On the "Viewer Protocol Policy" choose "Redirect HTTP to HTTPS" to redirect all HTTP requests to HTTPS.</br><img src="/resources/aws/cloudfront/cloudfront-https-only/step8.png"/>
9. On the "Viewer Protocol Policy" choose "HTTPS Only" so CloudFront allows viewers to access your content only if they're using HTTPS.</br><img src="/resources/aws/cloudfront/cloudfront-https-only/step9.png"/>
10. Repeat the steps number 5 , 6 and 7 to verify if any other CloudFront Distribution is using HTTP-only listeners.</br>
