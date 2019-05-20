[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Default VPC In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default VPC In Use |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determines whether the default VPC is being used for launching EC2 instances. |
| **More Info** | The default VPC should not be used in order to avoid launching multiple services in the same network which may not require connectivity. Each application, or network tier, should use its own VPC. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/default-vpc.html |
| **Recommended Action** | Move resources from the default VPC to a new VPC created for that application or resource group. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/default-vpc-in-use/step2.png"/>
3. Scroll down the left navigation panel and choose "Your VPC" under "VPC Dashboard". </br> <img src="/resources/aws/ec2/default-vpc-in-use/step3.png"/>
4. Copy the default "VPC ID" from the "VPC" dashboard.</br>  <img src="/resources/aws/ec2/default-vpc-in-use/step4.png"/>
5. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/default-vpc-in-use/step5.png"/>
6. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/default-vpc-in-use/step6.png"/>
7. Click inside the " Filter by tags and attributes or search by keyword box" and paste the "VPC ID" we copied in Step4 and press "Enter". AWS console will return one or more EC2 instances using "default VPC".</br> <img src="/resources/aws/ec2/default-vpc-in-use/step7.png"/>
8. Repeat steps number 2 - 6 to check other AWS regions. </br>
9. Navigate to "VPC Dashboard" and choose "Your VPC" and click on the "Create VPC" button at the top panel. </br> <img src="/resources/aws/ec2/default-vpc-in-use/step9.png"/>
10. Inside "Create VPC" dialog box provide a name to the new VPC and within IPv4 CIDR block box, specify an IPv4 address range for the new VPC. Select the "IPv6 CIDR block" and "Tenancy" option as per the application requirement and click on the "Create" button at the bottom to create a new VPC. </br> <img src="/resources/aws/ec2/default-vpc-in-use/step10.png"/>
11. Navigate to the "EC2 dashboard" and select the "EC2 Instance" which is on default VPC. Click on the "Actions" button at the top and choose "Image" to create an "Amazon Machine Image" of the selected Instance. </br> <img src="/resources/aws/ec2/default-vpc-in-use/step11.png"/>
12. Under the "Create Image" panel provide the "Image Name" and "Image Description" and click on the "Create Image" button at the bottom.</br> <img src="/resources/aws/ec2/default-vpc-in-use/step12.png"/>
13. Once the "AMI" is created click on the "Launch Instance" button at the top panel to create a new "Instance".</br> <img src="/resources/aws/ec2/default-vpc-in-use/step13.png"/>
14. Clcik on the "My AMIs" option and choose the "AMI".</br> <img src="/resources/aws/ec2/default-vpc-in-use/step14.png"/>
15. Provide the other necessary details for the new "EC2-Instance" and under the "Configuration Instance" choose the newly created "VPC" instead of default VPC.</br> <img src="/resources/aws/ec2/default-vpc-in-use/step15.png"/>
16. Click on the "Launch" button once reviewing the necessary configuration to launch the new "EC2-Instance". Once the new "EC2-Instance" is in healthy state remove the older "EC2-Instance" which is using the default VPC.</br>
