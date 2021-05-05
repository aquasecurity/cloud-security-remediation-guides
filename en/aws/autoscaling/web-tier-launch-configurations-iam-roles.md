[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Web-Tier Launch Configurations IAM Roles

## Quick Info

| | |
|-|-|
| **Plugin Title** | Web-Tier Launch Configurations IAM Roles |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that Web-Tier Auto Scaling launch configuration is configured to use a customer created IAM role. |
| **More Info** | Web-Tier Auto Scaling launch configuration should have a customer created Web-Tier IAM role to provide necessary credentials to access AWS services. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/us-iam-role.html |
| **Recommended Action** | Update Web-Tier Auto Scaling launch configuration and attach a customer created Web-Tier IAM role |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Launch Configurations" at the bottom.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step3.png"/>
4. On the "Launch Configuration" page, Select the Launch Configuration which needs to be checked for IAM role.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step4.png"/>
5. On the "Launch configurations" page, scroll down and under the Details check the value of the IAM Instance Profile.If the IAM Instance Profile is blank then the selected Launch Configuration group is not configured to use a customer created IAM role.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step5.png"/>
6. Repeat steps number 2 - 5 to check other groups in the account.</br>
7. Navigate to IAM dashboard at https://console.aws.amazon.com/iam/.</br>
8. In the "IAM dashboard", click on the "Roles" option at the left navigation panel.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step8.png"/>
9. Click on the "Create Role" button to create a new IAM role.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step9.png"/>
10. On the "Create role page", select type of trusted entity as "AWS" and and choose EC2 from Choose the service that will use this role list.Click on the next "Permissions" button.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step10.png"/>
11. On the "Permissions" panel, select the "AmazonEC2FullAccess", select one or more policies from the list, then click Next: Tags button to continue the setup process.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step11.png"/>
12. On the "Add tags" page, add the tag as per the requirement and  click on the "Next: Review" button.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step12.png"/>
13. Enter the "Role Name" and click on the "Create Role" button to complete the process.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step13.png"/>
14. Navigate to EC2 dashboard at https://console.aws.amazon.com/ec2/.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step14.png"/>
15. In the left navigation panel, choose "Launch Configuration" and select the ASG launch configuration that need to modify.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step15.png"/>
16. On the "Launch Configuration" page, scroll down and click on the "Copy launch configuration" button.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step16.png"/>
17. On the "Create launch configuration" page, scroll down and select the "IAM instance profile" from the dropdown under the Additional configuration.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step17.png"/>
18. Click on the "Create launch configuration" button at the bottom to make the changes.</br> <img src="/resources/aws/autoscaling/web-tier-launch-configurations-iam-roles/step18.png"/>
19. Repeat steps number 8 - 18 to update Web-Tier Auto Scaling launch configuration and attach a customer created App-Tier IAM role.</br>



