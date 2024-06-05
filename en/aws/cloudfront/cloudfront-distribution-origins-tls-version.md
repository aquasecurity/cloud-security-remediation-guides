# AWS / CloudFront / CloudFront Distribution Origins TLS Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Distribution Origins TLS Version |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure CloudFront Distribution custom origin TLS version is not deprecated. |
| **More Info** | The TLS (Transport Layer Security) protocol secures transmission of data over the internet using standard encryption technology. Encryption should be set with the latest version of TLS where possible.  |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/secure-connections-supported-viewer-protocols-ciphers.html |
| **Recommended Action** | Modify cloudFront distribution and update the TLS version. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the left navigation panel, under CloudFront, choose Distributions.
4. Click the name of the CloudFront distribution that you want to Edit.
5. Select the Origins tab. 
6. Select the distribution origin that you want to reconfigure then click Edit.
7. Select the latest supported version of TLS from the Minimum Origin SSL protocol list.</br> <img src="/resources/aws/cloudfront/cloudfront-distribution-origins-tls-version/step7.png"/>
8. Click Save changes.
