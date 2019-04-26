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
2. Select the "Services" option and search for CloudFront. </br>
3. Select the "CloudFront Distribution" that needs to be verified.</br> 
4. Click the "Distribution Settings" button from Menu to get into the "CloudFront Distribution" configuration page. </br>
5. Click the "Edit" button from the  General tab on the top menu. </br>
6. Choose the "Security Policy" that you want CloudFront to use for HTTPS connections and must use  TLSv1 or later to choose the Security Protocol.</br>

