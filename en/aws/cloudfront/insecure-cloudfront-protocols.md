[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / Insecure CloudFront Protocols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Insecure CloudFront Protocols |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Detects the use of insecure HTTPS SSL/TLS protocols for use with HTTPS traffic between viewers and CloudFront |
| **More Info** | CloudFront supports SSLv3 and TLSv1 protocols for use with HTTPS traffic, but only TLSv1.1 or higher should be used unless there is a valid business justification to support the older, insecure SSLv3. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/secure-connections-supported-viewer-protocols-ciphers.html |
| **Recommended Action** | Ensure that traffic sent between viewers and CloudFront is passed over HTTPS and uses TLSv1.1 or higher. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront/insecure-cloudfront-protocols/step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that needs to be verified.</br> ![Step 3](/resources/aws/cloudfront/insecure-cloudfront-protocols/step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront/insecure-cloudfront-protocols/step4.png "Step 4 - Distribution Settings")
5. Click the "Edit" button from the  General tab on the top menu. </br>![Step 5](/resources/aws/cloudfront/insecure-cloudfront-protocols/step5.png "Step 5 - Edit")
6. Scroll down and choose the "Security Policy" that you want CloudFront to use for HTTPS connections and must use TLSv1.1 or higher SSL protocols.</br>![Step 6](/resources/aws/cloudfront/insecure-cloudfront-protocols/step6.png "Step 6 - Security Policy")
7. Scroll down and click on "Yes,Edit" to save the changes.</br>![Step 7](/resources/aws/cloudfront/insecure-cloudfront-protocols/step7.png "Step 7 - Edit")
8. Repeat the steps 5 and 6 to establish any other "CloudFront Distribution" is not using an insecure SSL protocol for HTTPS traffic.</br>
