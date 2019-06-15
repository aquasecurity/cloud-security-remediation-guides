[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SES / Email DKIM Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Email DKIM Enabled |
| **Cloud** | AWS |
| **Category** | SES |
| **Description** | Ensures DomainKeys Identified Mail (DKIM) is enabled for domains and addresses in SES. |
| **More Info** | DKIM is a security feature that allows recipients of an email to veriy that the sender domain has authorized the message and that it has not been spoofed. |
| **AWS Link** | http://docs.aws.amazon.com/ses/latest/DeveloperGuide/easy-dkim.html |
| **Recommended Action** | Enable DKIM for all domains and addresses in all regions used to send email through SES. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for SES. </br> <img src="/resources/aws/ses/email-dkim-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Domains/Email Addresses" under "Identity Management".</br> <img src="/resources/aws/ses/email-dkim-enabled/step3.png"/>
4. Select the identity either "Domains/Email Addresses" which needs to be verified and click on the "View Details" button at the top.</br> <img src="/resources/aws/ses/email-dkim-enabled/step4.png"/>
5. Scroll down the selected identity configuration page and click on the "DKIM". If "DKIM is not enabled for this email address" message is shown when the "DKIM" is not enabled for selected "Identity". An email message that is sent using DKIM includes a DKIM-Signature header field that contains a cryptographically signed representation of the message.</br> <img src="/resources/aws/ses/email-dkim-enabled/step5.png"/>
6. Repeat step number 2 - 5 to verify other identities either "Domains/Email Addresses".</br>
7. Navigate to "SES" and choose the identity either "Domains/Email Addresses" which needs to be enabled with "DKIM" and click on the "View Details" button at the top.</br> <img src="/resources/aws/ses/email-dkim-enabled/step7.png"/>
8. Scroll down the selected identity configuration page click "DKIM" tab to expand and click on the "Generate DKIM Settings" button.</br> <img src="/resources/aws/ses/email-dkim-enabled/step8.png"/>
9. Copy and paste the generated "CNAME" on the registered identity DNS zone file with the CNAME record information. Once the status is verified click on the "Enable" next to "DKIM" to enable the "DKIM" services. Verification process of these settings may take up to 72 hours.</br> <img src="/resources/aws/ses/email-dkim-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to enable DKIM for all domains and addresses in all regions used to send email through SES.</br>
