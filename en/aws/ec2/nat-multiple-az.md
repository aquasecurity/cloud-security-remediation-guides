[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / NAT Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | NAT Multiple AZ |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures managed NAT instances exist in at least 2 AZs for availability purposes |
| **More Info** | Creating NAT instances in a single AZ creates a single point of failure for all systems in the VPC. All managed NAT instances should be created in multiple AZs to ensure proper failover. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/vpc-nat-gateway.html |
| **Recommended Action** | Launch managed NAT instances in multiple AZs. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/nat-multiple-az/step2.png"/>
3. Scroll down the left navigation panel and choose "Your VPCs". Select the VPC that needs to be verified. </br> <img src="/resources/aws/ec2/nat-multiple-az/step3.png"/>
4. Scroll down the left navigation panel and choose "NAT Gateways". If there are only a single "NAT Gateway" then all the "EC2 Instances" within private subnet will share the same gateway. </br> <img src="/resources/aws/ec2/nat-multiple-az/step4.png"/>
5. On the "Details" tab under the "NAT Gateway" click on the subnet id link next to "Subnet" attribute to verify where the selected NAT gateway was created. </br> <img src="/resources/aws/ec2/nat-multiple-az/step5.png"/>
6. Check the "Availability Zone" to verify where the selected "NAT Gateway" subnets located. </br>  <img src="/resources/aws/ec2/nat-multiple-az/step6.png"/>
7. Repeat steps number 2 - 6 to verify "Availability Zone" for other "NAT Gateways" in the selected AWS region. </br> <img src="/resources/aws/ec2/nat-multiple-az/step7.png"/>
8. Navigate to "VPC Dashboard" and click on the "NAT Gateways" under the "Virtual Private Cloud" on the left navigation panel.</br> <img src="/resources/aws/ec2/nat-multiple-az/step8.png"/>
9. Click on the "Create NAT Gateway" button at the top panel to create a new "NAT Gateway" in different "Availabilty Zone".</br> <img src="/resources/aws/ec2/nat-multiple-az/step9.png"/>
10. On the "Create NAT Gateway" page select the "Subnet" from the dropdown menu and click on the "Create New EIP" button to assign a new Elastic IP to the "NAT Gateway".</br> <img src="/resources/aws/ec2/nat-multiple-az/step10.png"/>
11. Click on the "Create a NAT Gateway" button at the bottom to create a new "NAT Gateway".</br> <img src="/resources/aws/ec2/nat-multiple-az/step11.png"/>
12. On the successful creation of "NAT Gateway" following message will show: "Your NAT gateway has been created".</br> <img src="/resources/aws/ec2/nat-multiple-az/step12.png"/>
13. Repeat steps number 8 - 12 to create a "NAT Gateway" in a different "Availabilty Zone". </br>

