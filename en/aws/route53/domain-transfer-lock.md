[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Route53 / Domain Transfer Lock

## Quick Info

| | |
|-|-|
| **Plugin Title** | Domain Transfer Lock |
| **Cloud** | AWS |
| **Category** | Route53 |
| **Description** | Ensures domains have the transfer lock set |
| **More Info** | To avoid having a domain maliciously transferred to a third-party, all domains should enable the transfer lock unless actively being transferred. |
| **AWS Link** | http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/domain-transfer-from-route-53.html |
| **Recommended Action** | Enable the transfer lock for the domain |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Route53. </br> <img src="/resources/aws/route53/domain-transfer-lock/step2.png"/>
3. Scroll down the left navigation panel and choose "Registered Domains" under "Domains". </br> <img src="/resources/aws/route53/domain-transfer-lock/step3.png"/>
4. Select the "Domain" that needs to be verified for "Domain Transfer Lock". </br> <img src="/resources/aws/route53/domain-transfer-lock/step4.png"/>
5. Click pn the "Domain Name" as a link to access the configuration settings and under the "Registered doamins" check for "Transfer Lock" option. If "Transfer Lock" is set to "Disable" then the AWS cannot prevent an unauthorized transfer to another registrar.</br> <img src="/resources/aws/route53/domain-transfer-lock/step5.png"/>
6. Repeat steps number 2 - 5 to verify other domains in the region.</br>
7. Navigate to "Route53" and choose "Registered Domains" under "Domains" and click on the "Domain" that need to enable "Transfer Lock".</br> <img src="/resources/aws/route53/domain-transfer-lock/step7.png"/>
8. Click on the "Domain Name" as a link to access the configuration settings and click on the "Enable" option next to "Transfer Lock". "Transfer Lock" feature is now set to "Enabled". <img src="/resources/aws/route53/domain-transfer-lock/step8.png"/>
9. Repeat steps number 7 - 8 to enable the transfer lock for the domain.
