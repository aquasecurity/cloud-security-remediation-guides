[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open MySQL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open MySQL |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 4333 or 3306 for MySQL is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as MySQL should be restricted to known IP addresses. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Restrict TCP ports 4333 and 3306 to known IP addresses |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-mysql/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-mysql/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-mysql/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound rules". Verify the value for "Source" column for "MYSQL/Aurora" under "Type" for ports "3306 or 4333" and if any rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has "TCP" port for "MySQL" open to the public.</br> <img src="/resources/aws/ec2/open-mysql/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to be modified to restrict the access of "TCP" port "3306 or 4333" for "MySQL"  to specific IP address. </br> <img src="/resources/aws/ec2/open-mysql/step7.png"/>
8. Scroll down the page and select the "Inbound rules" and click on the "Edit inbound rules" button. </br> <img src="/resources/aws/ec2/open-mysql/step8.png"/>
9. In the "Edit inbound rules" tab select either the "MyIP" or "Custom" from the "Source" column.</br> <img src="/resources/aws/ec2/open-mysql/step9.png"/>
10. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow "MySQL" inbound traffic only from specific IP address.</br> <img src="/resources/aws/ec2/open-mysql/step10.png"/>
11. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements for "MySQL" and specify static IP/Elastic IP address along with "Description" for the "Security Group" rule. </br> <img src="/resources/aws/ec2/open-mysql/step11.png"/>
12. Click on the "Save rules" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-mysql/step12.png"/>
13. Repeat steps number 7 - 12 to restrict TCP port "3306 and 4333" for "MySQL" to known IP address.</br>
