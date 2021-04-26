[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ACM / ACM Certificate Expiry

## Quick Info

| | |
|-|-|
| **Plugin Title** | ACM Certificate Expiry |
| **Cloud** | AWS |
| **Category** | ACM |
| **Description** | Detect upcoming expiration of ACM certificates |
| **More Info** | Certificates that have expired will trigger warnings in all major browsers. AWS will attempt to automatically renew the certificate but may be unable to do so if email or DNS validation cannot be confirmed. |
| **AWS Link** | https://docs.aws.amazon.com/acm/latest/userguide/managed-renewal.html |
| **Recommended Action** | Ensure AWS is able to renew the certificate via email or DNS validation of the domain. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for ACM. </br> <img src="/resources/aws/acm/acm-certificate-expiry/step2.png"/>
3. Select the SSL/TLS certificate that needs to examine and click on the Show/Hide Details button.</br> <img src="/resources/aws/acm/acm-certificate-expiry/step3.png"/>
4. Inside the Details section, check the certificate expiration information. If the "Expires" shows within 30days, make sure to renew the certificate at earliest.</br> <img src="/resources/aws/acm/acm-certificate-expiry/step4.png"/>
5. Repeat steps number 2 - 4 to verify other "Amazon Certificates" in the selected AWS region.</br> 
6. Navigate to AWS ACM dashboard at https://console.aws.amazon.com/acm/ and select the SSL/TLS certificate that is expiring in less than 30 days.</br> <img src="/resources/aws/acm/acm-certificate-expiry/step6.png"/>
7. Select the check box next to the certificate that requires manual domain validation. Then choose Actions, Resend validation email to renew the certificate via email.</br> <img src="/resources/aws/acm/acm-certificate-expiry/step7.png"/>
8. Repeat steps no. 6 – 7 to ensure AWS is able to renew the certificate via email or DNS validation of the domain.</br>



