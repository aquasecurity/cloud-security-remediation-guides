[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Instance IAM Role

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance IAM Role |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EC2 instances are using an IAM role instead of hard-coded AWS credentials |
| **More Info** | IAM roles should be assigned to all instances to enable them to access AWS resources. Using an IAM role is more secure than hard-coding AWS access keys into application code. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-roles-for-amazon-ec2.html |
| **Recommended Action** | Attach an IAM role to the EC2 instance |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/instance-iam-role/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/instance-iam-role/step3.png"/>
4. Select the "EC2 Instance" that needs to be verified and scroll down and click on the "Description" tab. </br> <img src="/resources/aws/ec2/instance-iam-role/step4.png"/>
5. On the "Description" tab scroll down and check for "IAM role" attribute value. If no value has assigned then the selected "EC2 Instance" has no "IAM role" assigned. </br> <img src="/resources/aws/ec2/instance-iam-role/step5.png"/>
6. Repeat steps number 2 - 5 to cross check other "EC2 Instances" in the selected AWS region.</br>
7. Navigate to "IAM" dashboard using the "Services" option.</br> <img src="/resources/aws/ec2/instance-iam-role/step7.png"/>
8. Scroll down the left panel and choose "Roles".</br> <img src="/resources/aws/ec2/instance-iam-role/step8.png"/>
9. On the "Roles" page click on the "Create Role" button to create a new "IAM role".</br> <img src="/resources/aws/ec2/instance-iam-role/step9.png"/>
10. On the "Create Role" page choose the "AWS service", choose "EC2" and click on the "Next,Permission" button at the bottom. </br> <img src="/resources/aws/ec2/instance-iam-role/step10.png"/>
11. On a "Attach permissions policies" page search for "AmazonEC2FullAccess" policy from the "Filter policies" search bar which provides full access to all AWS EC2 services and resources. Click on the "Next:Tags" button to continue. </br> <img src="/resources/aws/ec2/instance-iam-role/step11.png"/>
12. On the "Add tags" provide a "Key" and "value" which can help to organize, track, or control access for the selected "IAM role". Click on the "Next:Review" button to continue the process. </br> <img src="/resources/aws/ec2/instance-iam-role/step12.png"/>
13. Provide a "Role name" and click on the "Create role" button to create the selected "IAM role".</br> <img src="/resources/aws/ec2/instance-iam-role/step13.png"/>
14. Navigate to "EC2" dashboard and select the "EC2 Instance" on which we need to attach the "IAM role".</br> <img src="/resources/aws/ec2/instance-iam-role/step14.png"/>
15. Click on the "Actions" button at the top to create an "Amazon Machine Image" of the selected "EC2 Instance". Click on the "Image" option under "Actions" dropdown menu and click on the "Create Image".</br> <img src="/resources/aws/ec2/instance-iam-role/step15.png"/>
16. On the "Create Image" dialog box provide a "Image Name" and "Image Description". Click on the "Create Image" button at the bottom to create the "Amazon Machine Image" of the selected "EC2 Instance".</br> <img src="/resources/aws/ec2/instance-iam-role/step16.png"/>
17. Once the "Amazon Machine Image" is ready click on the "Launch" button to create a new "EC2 Instance" from the image created.</br> <img src="/resources/aws/ec2/instance-iam-role/step17.png"/>
18. On the "Configure Instance Details" page scroll down and choose the newly created "IAM role" from the dropdown menu and click on the "Review and Launch" button to create a new "EC2 Instance" with "IAM role" attached. </br> <img src="/resources/aws/ec2/instance-iam-role/step18.png"/>
19. Once the new "EC2 Instance" is deployed and working fine, terminate the older "EC2 Instance".</br>



