# AWS / CloudFront / CloudFront Distribution Field-Level Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Distribution Field-Level Encryption |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure that field-level encryption is enabled for your Amazon CloudFront web distributions. |
| **More Info** | With Amazon CloudFront, you can enforce secure end-to-end connections to origin servers by using HTTPS. Field-level encryption adds an additional layer of security that lets you protect specific data throughout system processing so that only certain applications can see it. Field-level encryption allows you to enable users to securely upload sensitive information to web servers.  |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html |
| **Recommended Action** | Enable field-level encryption for CloudFront distributions. |

## Detailed Remediation Steps
1. [Create an RSA key pair](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html#field-level-encryption-setting-up-step1).
2. [Add your public key to CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html#field-level-encryption-setting-up-step2).
3. [Create a profile for field-level encryption](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html#field-level-encryption-setting-up-step3).
4. [Create a configuration](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html#field-level-encryption-setting-up-step4).
5. [Add a configuration to a cache behavior](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/field-level-encryption.html#field-level-encryption-setting-up-step5).