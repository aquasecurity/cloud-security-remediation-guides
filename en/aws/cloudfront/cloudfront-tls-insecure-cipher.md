# AWS / CloudFront / CloudFront TLS Insecure Cipher

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront TLS Insecure Cipher |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure CloudFront distribution TLS Version is not using insecure cipher. |
| **More Info** | The TLS (Transport Layer Security) protocol secures transmission of data over the internet using standard encryption technology. Encryption should be set with the latest version of TLS where possible. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/secure-connections-supported-viewer-protocols-ciphers.html |
| **Recommended Action** | Modify cloudFront distribution and update the TLS version. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the left navigation panel, under CloudFront, choose Distributions.
4. Click the name of the CloudFront distribution that you want to Edit.
5. Select the General tab, and Click Edit. </br> <img src="/resources/aws/cloudfront/cloudfront-tls-insecure-cipher/step5.png"/>
6. Under Security policy, Select the latest supported version of TLS.</br> <img src="/resources/aws/cloudfront/cloudfront-tls-insecure-cipher/step6.png"/>
7. Click Save changes.


