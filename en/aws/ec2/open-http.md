[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open HTTP

## Quick Info

| | |
|-|-|b b n
| **Plugin Title** | Open HTTP |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 80 for HTTPS is open to the public |
| **More Info** | Network security groups should be periodically evaluated for port misconfigurations. Where certain ports and protocols may be exposed to the Internet, they should be evaluated for necessity and restricted wherever they are not explicitly required and narrowly configured. |
| **AWS Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict TCP port 80 to known IP addresses. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-http/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-http/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-http/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound rules". Verify the value for "Source" column for "HTTP" under "Type" for port "80" if the rule have value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has "TCP" port for "HTTP" open to the public.</br> <img src="/resources/aws/ec2/open-http/step5.png"/>
6. Repeat step number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to be modified to restrict the access of "TCP" port "80" for "HTTP"  to specific IP address. </br> <img src="/resources/aws/ec2/open-http/step7.png"/>
8. Scroll down the page and select the "Inbound rules" and click on the "Edit inbound rules" button to the right. </br> <img src="/resources/aws/ec2/open-http/step8.png"/>
9. In the "Edit inbound rules" tab select either the "MyIP" or "Custom" from the "Source" column.</br> <img src="/resources/aws/ec2/open-http/step9.png"/>
10. In the "Edit inbound rules" tab select the "MyIP" or any CIDR Block from the "Source" column to allow "HTTP" inbound traffic only from your IP address.</br>  <img src="/resources/aws/ec2/open-http/step10.png"/>
11. Click on the "Save rules" button to make the necessary changes. </br>  <img src="/resources/aws/ec2/open-http/step11.png"/>
12. Repeat step number 7 - 12 to restrict TCP port "80" for "HTTP".</br>

