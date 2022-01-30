[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Certificate Expiry

## Quick Info

| | |
|-|-|
| **Plugin Title** | Certificate Expiry |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detect upcoming expiration of certificates used with ELBs |
| **More Info** | Certificates that have expired will trigger warnings in all major browsers |
| **AWS Link** | http://docs.aws.amazon.com/ElasticLoadBalancing/latest/DeveloperGuide/elb-update-ssl-cert.html |
| **Recommended Action** | Update your certificates before the expiration date |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/iam/access-keys-extra/step2.png"/>
3. In the left navigation panel, scroll down to "Load balancing" and click on "Load balancers". </br> <img src="/resources/aws/iam/access-keys-extra/step3.png"/>
4. Click on the search box at the top and select "Type" as the filter attribute and "application" as the type value. </br> <img src="/resources/aws/iam/access-keys-extra/step4.png"/>
5. This search will filter and return load balancers with application type only.</br> <img src="/resources/aws/iam/access-keys-extra/step5.png"/>
6. Select the load balancer and click on "Listeners" tab in the bottom panel. </br> <img src="/resources/aws/iam/access-keys-extra/step6.png"/>
7. Scroll down to "HTTPS : 443" listener ID and click on "View/edit certificates". </br> <img src="/resources/aws/iam/access-keys-extra/step7.png"/>
8. Check the date under the "Expires" column for the certificates listed. If the date is already passed or is near then you should renew the certificate by clicking on the "ACM" Link under "Service" column.</br> <img src="/resources/aws/iam/access-keys-extra/step8.png"/>
9. Repeat steps 5 to 8 for all other application load balancers.
