[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELB No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELB No Instances |
| **Cloud** | AWS |
| **Category** | ELB |
| **Description** | Detects ELBs that have no backend instances attached |
| **More Info** | All ELBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old ELBs with no instances present a security concern if new instances are accidentally attached. |
| **AWS Link** | http://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-backend-instances.html |
| **Recommended Action** | Delete old ELBs that no longer have backend resources. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> ![Step 2](/resources/aws/elb/elb-no-instances/step2.png "Step 2 - Services")
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> ![Step 3](/resources/aws/elb/elb-no-instances/step3.png "Step 3 - Load Balancers")
4. Select the "Load Balancer" which needs to be verified. </br> ![Step 4](/resources/aws/elb/elb-no-instances/step4.png "Step 4 - Load Balancer")
5. Select the "Instances" tab from the bottom panel and scroll down to "Edit Availability Zones" option.</br> ![Step 5](/resources/aws/elb/elb-no-instances/step5.png "Step 5 - Instances")
6. Scroll down and check for "Instances Count" under "Edit Availability Zones". If the load balancer "Instance Count" is 0 it means there are no registered Instances. </br> ![Step 6](/resources/aws/elb/elb-no-instances/step6.png "Step 6 - Instances") 
7. Select the unused "Load Balancer" and from "Action" tab from the top panel click on "Delete". </br> ![Step 7](/resources/aws/elb/elb-no-instances/step7.png "Step 7 - Delete") 
8. Click on "Yes,Delete" from the "Delete Load Balancer" panel. </br> </br> ![Step 8](/resources/aws/elb/elb-no-instances/step8.png "Step 8 - Delete") 
