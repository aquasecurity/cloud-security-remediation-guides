[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ACM / ACM Certificate Validation

## Quick Info

| | |
|-|-|
| **Plugin Title** | ACM Certificate Validation |
| **Cloud** | AWS |
| **Category** | ACM |
| **Description** | ACM certificates should be configured to use DNS validation. |
| **More Info** | With DNS validation, ACM will automatically renew certificates before they expire, as long as the DNS CNAME record is in place. |
| **AWS Link** | https://aws.amazon.com/blogs/security/easier-certificate-validation-using-dns-with-aws-certificate-manager/ |
| **Recommended Action** | Configure ACM managed certificates to use DNS validation. |

## Detailed Remediation Steps
1. Log in to the AWS console and search for "Certificate Manager".</br> <img src="/resources/aws/acm/acm-certificate-validation/step1.png"/>
2. Click into each certificate that has been requested. </br> <img src="/resources/aws/acm/acm-certificate-validation/step2.png"/>
3. Expand the domains associated with the certificate.</br> <img src="/resources/aws/acm/acm-certificate-validation/step3.png"/>
4. Ensure each domain listed has DNS validation configured. If DNS validation is used, DNS records will be listed for the domain and the type will be CNAME.</br> <img src="/resources/aws/acm/acm-certificate-validation/step4.png"/>
5. Ensure that the records provided by AWS are configured and valid within your DNS provider (such as Route 53).
6. If DNS validation is not used, request a new certificate for the same domains using DNS validation and update the downstream services to use this new certificate. Once done, delete the old certificate to ensure it can no longer be used.</br> <img src="/resources/aws/acm/acm-certificate-validation/step6.png"/>
