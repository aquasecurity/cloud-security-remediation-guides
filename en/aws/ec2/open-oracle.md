[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open Oracle

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Oracle |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 1521 for Oracle is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open         to the public to function properly, more sensitive services such as Oracle         should be restricted to known IP addresses. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Restrict TCP ports 1521 to known IP addresses |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-oracle/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-oracle/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-oracle/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound rules". Verify the value for "Source" column for "Oracle-RDS" under "Type" for port "1521" and if any rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has "TCP" port for "Oracle" open to the public.</br> <img src="/resources/aws/ec2/open-oracle/step5.png"/>
6. Repeat step number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to be modified to restrict the access of "TCP" port 1521 for "Oracle"  to specific IP address. </br> <img src="/resources/aws/ec2/open-oracle/step7.png"/>
8. Scroll down the page and select the "Inbound rules" and click on the "Edit inbound rules" button to the right. </br> <img src="/resources/aws/ec2/open-oracle/step8.png"/>
9. In the "Edit inbound rules" tab select either the "MyIP" or "Custom" from the "Source" column.</br> <img src="/resources/aws/ec2/open-oracle/step9.png"/>
10. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow "Oracle" inbound traffic only from your IP address.</br> <img src="/resources/aws/ec2/open-oracle/step10.png"/>
11. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements for "Oracle" and specify static IP/Elastic IP address along with "Description" for the "Security Group" rule. </br> <img src="/resources/aws/ec2/open-oracle/step11.png"/>
12. Click on the "Save rules" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-oracle/step12.png"/>
13. Repeat step number 7 - 12 to restrict "TCP" port "1521" for "Oracle" to known IP address.</br>
