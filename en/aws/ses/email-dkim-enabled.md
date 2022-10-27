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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for SES. </br> <img src="/resources/aws/ses/email-dkim-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Verified identities" under "Configuration".</br> <img src="/resources/aws/ses/email-dkim-enabled/step3.png"/>
4. Select the identity "Email Address" which needs to be verified and click on the "Identity".</br> <img src="/resources/aws/ses/email-dkim-enabled/step4.png"/>
5. In the identity configuration page, you will see this message at the top of the page "Verify ownership of this identity, check your inbox for a verification request email and click the link provided.</br> <img src="/resources/aws/ses/email-dkim-enabled/step5.png"/>
6. Once the email is verified via link provided your status will change to "Verified" on the "Verified identities" page.</br> <img src="/resources/aws/ses/email-dkim-enabled/step6.png"/>
7. Repeat step number 3 - 5 to verify all other Email Address identities.</br>
