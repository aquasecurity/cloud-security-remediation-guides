[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELBv2 / ELBv2 No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 No Instances |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Detects ELBs that have no target groups attached |
| **More Info** | All ELBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old ELBs with no target groups present a security concern if new target groups are accidentally attached. |
| **AWS Link** | https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html |
| **Recommended Action** | Delete old ELBs that no longer have backend resources. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elbv2/elbv2-no-instances/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elbv2/elbv2-no-instances/step3.png"/>
4. Select the "Load Balancer" which needs to be verified. </br> <img src="/resources/aws/elbv2/elbv2-no-instances/step4.png"/>
5. Select the "Instances" tab from the bottom panel and scroll down to "Edit Availability Zones" option.</br> <img src="/resources/aws/elbv2/elbv2-no-instances/step5.png"/>
6. Scroll down and check for "Instances Count" under "Edit Availability Zones". If the load balancer "Instance Count" is 0 it means there are no registered instances. </br> <img src="/resources/aws/elbv2/elbv2-no-instances/step6.png"/>
7. Select the unused "Load Balancer" and from "Action" tab from the top panel click on "Delete". </br> <img src="/resources/aws/elbv2/elbv2-no-instances/step7.png"/>
8. Click on "Yes,Delete" from the "Delete Load Balancer" panel. </br> </br> <img src="/resources/aws/elbv2/elbv2-no-instances/step8.png"/>
9. Repeat steps number 2 - 9 to delete old ELBs that no longer have backend resources.



