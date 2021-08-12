[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 Deletion Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 Deletion Protection |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensures ELBv2 load balancers are configured with deletion protection. |
| **More Info** | ELBv2 load balancers should be configured with deletion protection to prevent accidentaldeletion of live resources in production environments. |
| **AWS Link** | https://docs.aws.amazon.com/elasticloadbalancing/latest/application/application-load-balancers.html#deletion-protection |
| **Recommended Action** | Update ELBv2 load balancers to use deletion protection to prevent accidental deletion |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step3.png"/>
4. Select the "Load Balancer" which needs to be verified. </br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step4.png"/>
5. On the "Load Balancers" page, scroll down and check under the "Attributes" whether the "Delete Protection" is enabled or disabled.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step5.png"/>
6. Repeat steps number 2 - 5 to check other Load balancers in the account.</br>
7. Navigate to EC2 dashboard at https://console.aws.amazon.com/ec2/.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step7.png"/>
8. On the "EC2" dashboard, scroll down and select the "Load balancers" option from the left navigation panel and select the "Load balancer" in which "Delete Protection" needs to be enabled.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step8.png"/>
9. On the Description tab, choose Edit attributes.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step9.png"/>
10. On the Edit load balancer attributes page, select Enable for Delete Protection, and then choose Save.</br> <img src="/resources/aws/elbv2/elbv2-deletion-protection/step10.png"/>
11. Repeat steps number 7 - 10 to update ELBv2 load balancers to use deletion protection to prevent accidental deletion.</br>




