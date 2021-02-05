[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open Docker

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Docker |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if Docker port 2375 or 2376 is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as Docker should be restricted to known IP addresses. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Restrict TCP ports 2375 and 2376 to known IP addresses |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/open-docker/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Group" under "Network & Security".</br> <img src="/resources/aws/ec2/open-docker/step3.png"/>
4. Select the "EC2 Security Group" that needs to be verified. </br> <img src="/resources/aws/ec2/open-docker/step4.png"/>
5. Scroll down the bottom panel and choose "Inbound". Verify the value for "Source" column and if TCP rule for 'Docker Port' 2375 or 2376 has a value set to "0.0.0.0/0" or "::/0 " then the selected "Security Group" has Docker ports open to the public.</br> <img src="/resources/aws/ec2/open-docker/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Security Groups" in the selected AWS region.</br> 
7. Navigate to "Security Groups" under "Network & Security" and select the "Security Group" that needs to modify to restrict the access to specific ip address. </br> <img src="/resources/aws/ec2/open-docker/step7.png"/>
8. Scroll down the page and select the "Inbound" and click on the "Edit" button. </br> <img src="/resources/aws/ec2/open-docker/step8.png"/>
9. In the "Edit inbound rules" tab select the "MyIP" from the "Source" column to allow inbound traffic only from specific IP address for Docker ports.</br> <img src="/resources/aws/ec2/open-docker/step9.png"/>
10. In the "Edit inbound rules" tab select the "Custom" from the "Source" column as per the requirements and specify static IP/Elastic IP address of the permitted host along with "Description" for the "Security Group" rule for Docker Port. </br> <img src="/resources/aws/ec2/open-docker/step10.png"/>
11. Click on the "Save" button to make the necessary changes. </br> <img src="/resources/aws/ec2/open-docker/step11.png"/>
12. Repeat steps number 7 - 11 to restrict TCP ports 2375 and 2376 to known IP addresses.</br>



