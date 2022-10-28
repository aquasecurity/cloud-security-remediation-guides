[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open VNC Server

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open VNC Server |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 5900 for VNC Server is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as VNC Server should be restricted to known IP addresses. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Restrict TCP port 5900 to known IP addresses |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-vnc-server/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-vnc-server/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-vnc-server/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound rules". Verify the value for "Source" column for "Custom TCP" for port 5900 under "Type" and if any rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has "TCP" port for "VNC Server" open to the public.</br> <img src="/resources/aws/ec2/open-vnc-server/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to be modified to restrict the access of "TCP" port 5900 for "VNC Server"  to specific IP address. </br> <img src="/resources/aws/ec2/open-vnc-server/step7.png"/>
8. Scroll down the page and select the "Inbound rules" and click on the "Edit Inbound rules" button to the right. </br> <img src="/resources/aws/ec2/open-vnc-server/step8.png"/>
9. In the "Edit inbound rules" tab select either the "MyIP" or "Custom" from the "Source" column.</br> <img src="/resources/aws/ec2/open-vnc-server/step9.png"/>
10. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow "VNC Server" inbound traffic only from your IP address.</br> <img src="/resources/aws/ec2/open-vnc-server/step10.png"/>
11. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements for "VNC Server" and specify static IP/Elastic IP address along with "Description" for the "Security Group" rule. </br> <img src="/resources/aws/ec2/open-vnc-server/step11.png"/>
12. Click on the "Save rules" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-vnc-server/step12.png"/>
13. Repeat steps number 7 - 12 to restrict TCP port 5900 for "VNC Server" to known IP address.</br>
