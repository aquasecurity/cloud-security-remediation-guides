[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / ELB Health Check Active

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELB Health Check Active |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures all Auto Scaling groups have ELB health check active. |
| **More Info** | Auto Scaling groups should have ELB health checks active to replace unhealthy instances in time. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-add-elb-healthcheck.html |
| **Recommended Action** | Enable ELB health check for the Auto Scaling groups. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/elb-health-check-active/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step3.png"/>
4. On the "Auto Scaling groups" page, select the auto scaling group which needs to be verified whether all Auto Scaling groups have ELB health check active or not.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step4.png"/>
5. On the "Auto Scaling groups" page, scroll down and check the "Health Check" and if the "Health Check Type" is showing as EC2 then the selected Auto Scaling group don't have ELB health check active.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step5.png"/>
6. Repeat steps number 2 - 5 to check other Auto Scaling group in the account.</br>
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Scroll down the EC2 console page, select the Auto Scaling group which needs to have ELB health check active.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step8.png"/>
9. Scroll down the "Auto Scaling group" page, on the "Health checks" tab, click on the "Edit" button.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step9.png"/>
10. On the "Health checks" page, click on the checkbox next to the "ELB" under the "Health check type" and click on the "Update" button to make the changes.</br> <img src="/resources/aws/autoscaling/elb-health-check-active/step10.png"/>
11. Repeat steps number 7 - 10 to enable ELB health check for the Auto Scaling groups.



