[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Excessive Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Security Groups |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if there are an excessive number of security groups in the account |
| **More Info** | Keeping the number of security groups to a minimum helps reduce the attack surface of an account. Rather than creating new groups with the same rules for each project, common rules should be grouped under the same security groups. For example, instead of adding port 22 from a known IP to every group, create a single "SSH" security group which can be used on multiple instances. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Limit the number of security groups to prevent accidental authorizations |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/excessive-security-groups/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Groups" under "Network & Security".</br>  <img src="/resources/aws/ec2/excessive-security-groups/step3.png"/>
4. Check the total number of "Security Groups" at the top right corner available in the selected AWS region. </br>  <img src="/resources/aws/ec2/excessive-security-groups/step4.png"/>
5. Repeat steps number 2 - 4 to check the "Security Group" threshold value for other regions. If the total number of running "Security Group" provisioned in your AWS account is greater than 50, the recommended threshold was exceeded. AWS has different threshold values as well depends on the region. </br>
6. Scroll down the left navigation panel and choose "Security Groups" under "Network & Security" and select the unnecessary/unused "Security Groups" that needs to be removed.</br>  <img src="/resources/aws/ec2/excessive-security-groups/step6.png"/>
7. Click on the "Actions" button at the top and click on the "Delete Security Groups" option. </br>  <img src="/resources/aws/ec2/excessive-security-groups/step7.png"/>
8. In the "Delete Security Groups" tab click on the "Yes,Delete" button to delete the selected "Security Groups".</br>  <img src="/resources/aws/ec2/excessive-security-groups/step8.png"/>
9. Repeat steps number 6 - 8 to remove unused "Security Groups" to prevent accidental authorizations. </br>
