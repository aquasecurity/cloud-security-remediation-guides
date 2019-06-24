[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Route53 / Domain Auto Renew

## Quick Info

| | |
|-|-|
| **Plugin Title** | Domain Auto Renew |
| **Cloud** | AWS |
| **Category** | Route53 |
| **Description** | Ensures domains are set to auto renew through Route53 |
| **More Info** | Domains purchased through Route53 should be set to auto renew. Domains that are not renewed can quickly be acquired by a third-party and cause loss of access for customers. |
| **AWS Link** | http://docs.aws.amazon.com/Route53/latest/APIReference/api-enable-domain-auto-renew.html |
| **Recommended Action** | Enable auto renew for the domain |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Route53. </br> <img src="/resources/aws/route53/domain-auto-renew/step2.png"/>
3. Scroll down the left navigation panel and choose "Registered Domains" under "Domains". </br> <img src="/resources/aws/route53/domain-auto-renew/step3.png"/>
4. Select the "Domain" that needs to be verified for "Domain Auto renew". </br> <img src="/resources/aws/route53/domain-auto-renew/step4.png"/>
5. Click pn the "Domain Name" as a link to access the configuration settings and under the "Registered doamins" check for "Auto Renew" option. If "Auto renew" is set to "Disable" then the AWS will not automatically renew the registration for the selected domain before the expiration date.</br> <img src="/resources/aws/route53/domain-auto-renew/step5.png"/>
6. Repeat steps number 2 - 5 to verify other domains in the region.</br>
7. Navigate to "Route53" and choose "Registered Domains" under "Domains" and click on the "Domain" that need to enable "Auto renew".</br> <img src="/resources/aws/route53/domain-auto-renew/step7.png"/>
8. Click on the "Domain Name" as a link to access the configuration settings and click on the "Enable" option next to "Auto renew". "Auto renew" feature is now set to "Enabled".</br> <img src="/resources/aws/route53/domain-auto-renew/step8.png"/>
9. Repeat steps number 7 - 8 to enable auto renew for the domain.</br>
