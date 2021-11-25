[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Detect EC2 Classic Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | Detect EC2 Classic Instances |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures AWS VPC is being used for instances instead of EC2 Classic |
| **More Info** | VPCs are the latest and more secure method of launching AWS resources. EC2 Classic should not be used. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Introduction.html |
| **Recommended Action** | Migrate instances from EC2 Classic to VPC |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step2.png"/>
3. On the EC2 dashboard, check the "Account Attributes".If the supported platform status set to VPC and EC2, then the selected account support both EC2-Classic and EC2-VPC platforms.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step3.png"/>
4.  Select the "Instances" option on the left navigation panel to verify whether any instances are lunch under "EC2-Classic."</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step4.png"/>
5. Select the "EC2 instance" and select the "Description" tab from the bottom panel. If the "VPC Id" parameter has no value assigned, the selected EC2 instance was launched within the EC2-Classic.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "EC2 instances" in the selected region.</br>
7. Navigate to "Instances" under the EC2 dashboard and copy all the Security Group settings of your selected instance.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step7.png"/>
8. Select the "EC2-Classic" instance and select the "Action" button from the top menu. Select the "Image" option and select the "Create Image" to create the AMI of the selected "EC2-Classic" Instance.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step8.png"/>
9. On the "Create Image" tab enter the Image Name and Image Description and click on the "Create Image" option at the bottom to make the changes.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step9.png"/>
10. Navigate to "AMIs" under "Images" and once the AMI is ready, select the "EC2-Classic" AMI and click on the "Launch" button at the top.</br></br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step10.png"/>
11. Select the "Instance Type" as per the requirement and click on the "Next: Configure Instance Details" button at the bottom.</br><img src="/resources/aws/ec2/detect-ec2-classic-instances/step11.png"/>
12. On the "Configure Instance Details" page, select the "VPC" option under Network and make other changes as per requirement. Click on the "Next: Add Storage" button at the bottom and select the "Storage" as per the need.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step12.png"/>
13. On the "Security Group" page, enter the same rules which we copied in Step7 and click on the "Review and Lunch" button. </br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step13.png"/>
14. Click on the "View Instances" option to return to the Instance page and check whether the new EC2-VPC instance have clear all the status check and is healthy and working fine.</br> <img src="/resources/aws/ec2/detect-ec2-classic-instances/step14.png"/>
15. Once the new EC2-VPC instance is working fine, terminate the older EC2-Classic instance.
16. Repeat steps number 7 - 15 to migrate instances from EC2 Classic to VPC.</br>
