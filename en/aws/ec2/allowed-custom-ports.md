[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Allowed Custom Ports

## Quick Info

| | |
|-|-|
| **Plugin Title** | Allowed Custom Ports |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that security groups does not allow public access to any port. |
| **More Info** | Security groups should be used to restrict access to ports from known networks. |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html |
| **Recommended Action** | Modify the security group to ensure the ports are not exposed publicly |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-custom-ports/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-custom-ports/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-custom-ports/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound". Verify the value for "Custom ports" opened and if any rule has a value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" as per not the AWS best practices.</br> <img src="/resources/aws/ec2/open-custom-ports/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Custom Port" that needs to modify to restrict the access to specific ip address. </br> <img src="/resources/aws/ec2/open-custom-ports/step7.png"/>
8. Scroll down the page and select the "Inbound" and click on the "Edit" button. </br> <img src="/resources/aws/ec2/open-custom-ports/step8.png"/>
9. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow inbound traffic only from specific IP address.</br> <img src="/resources/aws/ec2/open-custom-ports/step9.png"/>
10. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements and specify static IP/Elastic IP address of the permitted host along with "Description" for the "Security Group" rule. </br> <img src="/resources/aws/ec2/open-custom-ports/step10.png"/>
11. Click on the "Save" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-custom-ports/step11.png"/>
12. Repeat steps number 7 - 11 to modify the security group to to ensure the defined custom ports are not exposed publicly.</br>




