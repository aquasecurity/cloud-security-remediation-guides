[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Launch Configuration Referencing Missing Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Launch Configuration Referencing Missing Security Groups |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that Auto Scaling launch configurations are not utilizing missing security groups. |
| **More Info** | Auto Scaling launch configuration should utilize an active security group to ensure safety of managed instances. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/GettingStartedTutorial.html |
| **Recommended Action** | Ensure that the launch configuration security group has not been deleted. If so, remove it from launch configurations |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Launch Configurations" at the bottom.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step3.png"/>
4. On the "Launch Configuration" page, scroll down and copy the Security Groups attribute value.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step4.png"/>
5. Click on the "Security Group" name showing as a link to check whether the attached Security group exist or not.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step5.png"/>
6. If the "Security group" page is displaying the message that "The security group 'sg-000' does not exist" then the Auto Scaling launch configurations are utilizing missing security groups.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step6.png"/>
7. Repeat steps number 2 - 7 to check other groups in the account.</br>
8. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
9. In the left navigation panel, choose "Launch Configuration" and select the ASG launch configuration that need to modify.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step9.png"/>
10. On the "Launch Configuration" page, scroll down and click on the "Copy launch configuration" button.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step10.png"/>
11. On the "Create launch configuration" page, scroll down and select the "Create a new Security group" option and open the Inbound ports as per the requirements.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step11.png"/>
12. Click on the "Create launch configuration" button at the bottom to make the changes.</br> <img src="/resources/aws/autoscaling/launch-configuration-referencing-missing-security-groups/step12.png"/>
13. Repeat steps number 8 - 12 to ensure that the launch configuration security group has not been deleted.</br> 
