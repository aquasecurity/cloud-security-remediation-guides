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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step2.png"/>
3. Select the "CloudFront Distribution" that needs to be verified and click on it to open its configuration settings.</br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step3.png"/>
4. Click the "Behaviors" tab, select the "Behavior" which needs to be verified and click "Edit" </br><img src="/resources/aws/cloudfront/cloudfront-https-only/step4.png"/>
5. On the Edit Behavior page scroll down to "Viewer" Settings, verify the "Viewer Protocol Policy" and if "HTTP and HTTPS" is selected than CloudFront allows viewers to access your web content using either HTTP or HTTPS. </br> <img src="/resources/aws/cloudfront/cloudfront-https-only/step5.png"/>
6. To redirect all HTTP traffic to HTTPS under the "Viewer Protocol Policy" choose "Redirect HTTP to HTTPS" to redirect all HTTP requests to HTTPS.</br><img src="/resources/aws/cloudfront/cloudfront-https-only/step6.png"/>
7. If you want to drop all HTTP traffic then under the "Viewer Protocol Policy" choose "HTTPS Only" so CloudFront allows viewers to access your content only if they're using HTTPS.</br><img src="/resources/aws/cloudfront/cloudfront-https-only/step7.png"/>
8. Repeat the steps number 3 to 7 to verify if any other CloudFront Distribution is using HTTP-only listeners.</br>
