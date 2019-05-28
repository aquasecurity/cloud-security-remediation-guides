[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open All Ports Protocols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open All Ports Protocols |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if security group has all ports or protocols open to the public |
| **More Info** | Security groups should be created on a per-service basis and avoid allowing all ports or protocols. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Modify the security group to specify a specific port and protocol to allow. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-all-ports-protocols/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound". Verify the value for "Source" column and if any rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has one or many ports open to the public.</br> <img src="/resources/aws/ec2/open-all-ports-protocols/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to modify to restrict the access to specific ip address. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step7.png"/>
8. Scroll down the "Security Group" page and select the "Inbound" and click on the "Edit" button. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step8.png"/>
9. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow inbound traffic only from specific IP address.</br> <img src="/resources/aws/ec2/open-all-ports-protocols/step9.png"/>
10. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements and specify the "static IP" address of the permitted host along with "Description" for the "Security Group" rule. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step10.png"/>
11. Click on the "Save" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-all-ports-protocols/step11.png"/>
12. Repeat steps number 7 - 11 to modify the security group to specify a specific port and protocol to allow.</br>
