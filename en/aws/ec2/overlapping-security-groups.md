[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Overlapping Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Overlapping Security Groups |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if EC2 instances have security groups that share the same rules |
| **More Info** | Overlapping security group rules make managing EC2 instance access much more difficult. If a rule is removed from one security group, the access may still remain in another, resulting in unintended access to the instance. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Structure security groups to provide a single category of access and do not duplicate rules across groups used by the same instances. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/overlapping-security-groups/step2.png"/>
3. Scroll down the left navigation panel and choose "Security Groups" under "Network & Security". </br>  <img src="/resources/aws/ec2/overlapping-security-groups/step3.png"/>
4. Select the "Security Group" that needs to be verified and scroll down and click on the "Details" tab and copy "Security group ID". </br> <img src="/resources/aws/ec2/overlapping-security-groups/step4.png"/>
5. Scroll down the left navigation panel and choose "Instances" and search the copied "Security Group ID" copied above.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step5.png"/>
6. Check the number of "EC2 Instance(s)" using the Security Group and if there are more than 1 instances sharing the same "Security Group" then it's not according to the standard practice of AWS.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "EC2 Instances" using same "Security Group".</br>
8. Navigate to "Security Group" under "Network & Security" and click on the "Create Security Group" at the top.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step8.png"/>
9. On the "Create Security Group" panel provide a "Security Group Name" and "Description" for the new "Security Group".Select the "VPC" to which "Security Group" belongs.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step9.png"/>
10. Select the "Inbound Traffic Rules" by clicking on the "Add Rule" button and select the "Protocols" as per the requirement.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step10.png"/>
11. Click on the "Create security group" button at the bottom to create a new "Security Group". </br> <img src="/resources/aws/ec2/overlapping-security-groups/step11.png"/>
12. Navigate to "Instances" in the left panel and select the "Instance(s)" which are sharing the same "Security Group". Click on the "Actions" button at the top and click on the "Change security groups" under "Security".</br> <img src="/resources/aws/ec2/overlapping-security-groups/step12.png"/>
13. On the "Change Security Groups" tab select the new "Security Group" under "Associated security groups" and click on "Add security group" button.</br> <img src="/resources/aws/ec2/overlapping-security-groups/step13.png"/>
14. Click on the "Save" button to assign the selected "Security Group" to the "EC2 Instance".</br> <img src="/resources/aws/ec2/overlapping-security-groups/step14.png"/>
15. Remove any security group which may not be needed as required from the instance.
16. Repeat steps number 8 - 15 to structure security groups and to avoid their overlapping in "EC2 Instances".</br>
