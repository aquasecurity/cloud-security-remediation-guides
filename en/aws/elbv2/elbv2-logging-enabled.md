[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 Logging Enabled |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensures load balancers have request logging enabled. |
| **More Info** | Logging requests to ELB endpoints is a helpful way of detecting and investigating potential attacks, malicious activity, or misuse of backend resources.Logs can be sent to S3 and processed for further analysis. |
| **AWS Link** | http://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-access-logs.html |
| **Recommended Action** | Enable ELB request logging |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step3.png"/>
4. Select the "Load Balancer" which needs to be verified. </br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step4.png"/>
5. On the "Load Balancers" page, scroll down and check under the "Attributes" whether the "Access logs" is enabled or disabled.</br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other Load balancers in the account.</br>
7. Navigate to EC2 dashboard at https://console.aws.amazon.com/ec2/.</br> 
8. On the "EC2" dashboard, scroll down and select the "Load balancers" option from the left navigation panel and select the "Load balancer" in which "Access logs" needs to be enabled.</br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step8.png"/>
9. On the Description tab, choose Edit attributes.</br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step9.png"/>
10. For Access logs, select "Enable" and for S3 location, enter the name of your S3 bucket, including any prefix. If the bucket does not exist, choose Create this location for me. You must specify a name that is unique across all existing bucket names in Amazon S3 and follows the DNS naming conventions. Click on the Save button to make the changes.</br> <img src="/resources/aws/elbv2/elbv2-logging-enabled/step10.png"/>
11. Repeat steps number 7 - 10 to enable ELB request logging.</br>
