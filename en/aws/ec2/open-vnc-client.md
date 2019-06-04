[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open VNC Client

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open VNC Client |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 5500 for VNC Client is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as VNC Client should be restricted to known IP addresses. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Restrict TCP port 5500 to known IP addresses |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-vnc-client/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-vnc-client/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-vnc-client/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound". Verify the value for "Source" column for "Custom TCP Rule" for port 5500 under "Type" and if any rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has "TCP" port for "VNC Client" open to the public.</br> <img src="/resources/aws/ec2/open-vnc-client/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to modify to restrict the access of "TCP" port 5500 for "VNC Client"  to specific ip address. </br> <img src="/resources/aws/ec2/open-vnc-client/step7.png"/>
8. Scroll down the page and select the "Inbound" and click on the "Edit" button. </br> <img src="/resources/aws/ec2/open-vnc-client/step8.png"/>
9. In the "Edit inbound rules" tab select either the "MyIP" or "Custom" from the "Source" column.</br>  <img src="/resources/aws/ec2/open-vnc-client/step9.png"/>
10. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow "VNC Client" inbound traffic only from specific IP address.</br>  <img src="/resources/aws/ec2/open-vnc-client/step10.png"/>
11. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements for "VNC Client" and specify static IP/Elastic IP address along with "Description" for the "Security Group" rule. </br>  <img src="/resources/aws/ec2/open-vnc-client/step11.png"/>
12. Click on the "Save" button to make the necessary changes. </br>  <img src="/resources/aws/ec2/open-vnc-client/step12.png"/>
13. Repeat steps number 7 - 12 to restrict TCP port 5500 for "VNC Client" to known IP address.</br>
