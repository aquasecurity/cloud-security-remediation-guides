[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Default Security Group

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default Security Group |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure the default security groups block all traffic by default |
| **More Info** | The default security group is often used for resources launched without a defined security group. For this reason, the default rules should be to block all traffic to prevent an accidental exposure. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-network-security.html#default-security-group |
| **Recommended Action** | Update the rules for the default security group to deny all traffic by default |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/default-security-group/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/default-security-group/step3.png"/>
4. Select the "Instance" that needs to be verified and click on its name from the "Name" column.</br> <img src="/resources/aws/ec2/default-security-group/step4.png"/>
5. Scroll down the page and under "Security" check for "Security Groups". If the "Security Groups" is set to "default" then the EC2 network configuration is not following AWS security best practices.</br> <img src="/resources/aws/ec2/default-security-group/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "EC2 Instances".</br>
7. Scroll down the left navigation panel and choose "Security Groups" under "Network & Security".</br> <img src="/resources/aws/ec2/default-security-group/step7.png"/>
8. Click on the "Create security group" to create a new group as per our "EC2 Instance" requirements.</br> <img src="/resources/aws/ec2/default-security-group/step8.png"/>
9. Provide a name to the "Security Group" and select the "Inbound" and "Outbound" traffic rules as per the requirements.</br> <img src="/resources/aws/ec2/default-security-group/step9.png"/>
10. Click on the "Create security group" button at the bottom of the "Create Security Group" page to create the new security group.</br> <img src="/resources/aws/ec2/default-security-group/step10.png"/>
11. Scroll the left navigation panel and choose "Instances".</br> 
12. Select the "EC2 Instance" whose "Security Group" needs to be updated.</br> <img src="/resources/aws/ec2/default-security-group/step12.png"/>
13. Click on the "Actions" button at the top and click on "Security" and choose the "Change security group" option.</br> <img src="/resources/aws/ec2/default-security-group/step13.png"/>
14. Click on the search box under "Associated security groups" section and choose the newly created security group from the dropdown.</br> <img src="/resources/aws/ec2/default-security-group/step14.png"/>
15. Click on "Add security group" to the selected "EC2 Instance".</br> <img src="/resources/aws/ec2/default-security-group/step15.png"/>
16. Remove any other security group as needed by clicking on "Remove" button under "Security groups associated with the network interface". </br> <img src="/resources/aws/ec2/default-security-group/step16.png"/>
17. Repeat steps number 8 - 16 to update the "Security Group" as per the requirements.</br>
