[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / Insecure CloudFront Protocols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Insecure CloudFront Protocols |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Detects the use of insecure HTTPS SSL/TLS protocols for use with HTTPS traffic between viewers and CloudFront |
| **More Info** | CloudFront supports SSLv3 and TLSv1 protocols for use with HTTPS traffic, but only TLSv1 should be used unless there is a valid business justification to support the older, insecure SSLv3. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/secure-connections-supported-viewer-protocols-ciphers.html |
| **Recommended Action** | Ensure that traffic sent between viewers and CloudFront is passed over HTTPS and uses TLSv1, not SSLv3. |

## Detailed Remediation Steps

