[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Route53 / Domain Expiry

## Quick Info

| | |
|-|-|
| **Plugin Title** | Domain Expiry |
| **Cloud** | AWS |
| **Category** | Route53 |
| **Description** | Ensures domains are not expiring too soon |
| **More Info** | Expired domains can be lost and reregistered by a third-party. |
| **AWS Link** | http://docs.aws.amazon.com/Route53/latest/DeveloperGuide/registrar.html |
| **Recommended Action** | Reregister the expiring domain |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Route53. </br> <img src="/resources/aws/route53/domain-expiry/step2.png"/>
3. Scroll down the left navigation panel and choose "Registered Domains" under "Domains". </br> <img src="/resources/aws/route53/domain-expiry/step3.png"/>
4. Select the "Domain" that needs to be verified for "Domain Expiry". </br> <img src="/resources/aws/route53/domain-expiry/step4.png"/>
5. Click pn the "Domain Name" as a link to access the configuration settings and under the "Registered doamins" check for "Expires on" option. If the selected "Domain" is about to expire then take necessary steps for "Domain renewal".</br> <img src="/resources/aws/route53/domain-expiry/step5.png"/>
6. Repeat steps number 2 - 5 to verify other domains in the region.</br>
7. Navigate to "Route53" and choose "Registered Domains" under "Domains" and click on the "Domain" that need to be updated.</br> <img src="/resources/aws/route53/domain-expiry/step7.png"/>
8. Click on the "Domain Name" as a link to access the configuration settings and click on the "Enable" option next to "Auto renew". "Auto renew" feature is now set to "Enabled" and it will automatically renew the the "Domain" which is about to expire.</br> <img src="/resources/aws/route53/domain-expiry/step8.png"/>
9. If the "Domain" is already expired we need to contact Amazon Support for reregistering of the domain which also depends on the availabilty. For contacting Amazon Support please follow the below steps. </br>
10. Click on the "Support" option at the top panel to access the AWS support.</br> <img src="/resources/aws/route53/domain-expiry/step10.png"/>
11. Click on the "Create case" button to open a new support case under "My Support cases".</br> <img src="/resources/aws/route53/domain-expiry/step11.png"/>
12. Select "Account and billing support" and under and "Case classification" please select the "Type" as "Billing" and "Category" as "Domain name registration issue".</br> <img src="/resources/aws/route53/domain-expiry/step12.png"/>
13. Scroll down the page and provide the "Subject" as "Domain Reregistraion" and provide necessary details such as "Domain name" for reregistration along with "Account Id".</br> <img src="/resources/aws/route53/domain-expiry/step13.png"/>
14. Select the "Contact option" to communicate with AWS support of the choice and click on the "Submit" button to open the support case.</br> <img src="/resources/aws/route53/domain-expiry/step14.png"/>
15. Repeat steps number 7 - 14 for reregistration of the expiring domain.</br>
