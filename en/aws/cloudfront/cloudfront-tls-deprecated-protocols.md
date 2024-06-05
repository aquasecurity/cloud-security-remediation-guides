# AWS / CloudFront / CloudFront TLS Deprecated Protocols

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront TLS Deprecated Protocols |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensures AWS CloudFront distribution is not using deprecated TLS Version. |
| **More Info** | Use latest TLS policy for CloudFront distribution to meet compliance and regulatory requirements within your organisation and to adhere to AWS security best policies. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2020/07/cloudfront-tls-security-policy/ |
| **Recommended Action** | Modify cloudFront distribution and update the TLS version. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the left navigation panel, under CloudFront, choose Distributions.
4. Click the name of the CloudFront distribution that you want to Edit.
5. Select the General tab, and Click Edit. </br> <img src="/resources/aws/cloudfront/cloudfront-tls-deprecated-protocols/step5.png"/>
6. Under Security policy, Select the latest supported version of TLS.</br> <img src="/resources/aws/cloudfront/cloudfront-tls-deprecated-protocols/step6.png"/>
7. Click Save changes.


