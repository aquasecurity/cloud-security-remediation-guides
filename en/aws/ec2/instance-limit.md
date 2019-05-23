[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Instance Limit

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Limit |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if the number of EC2 instances is close to the AWS per-account limit |
| **More Info** | AWS limits accounts to certain numbers of resources. Exceeding those limits could prevent resources from launching. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html#using-instance-addressing-limit |
| **Recommended Action** | Contact AWS support to increase the number of instances available |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/instance-limit/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/instance-limit/step3.png"/>
4. Check the total number of EC2 instances at the top right corner available in the selected AWS region. </br> <img src="/resources/aws/ec2/instance-limit/step4.png"/>
5. Repeat steps number 2 - 4 to check the threshold value for other regions. If the total number of running EC2 instances provisioned in your AWS account is greater than 50, the recommended limit was exceeded. AWS has different threshold values as well depends on the region. Raise an AWS support ticket to limit the number of instances as per the requirements. </br>
6. Scroll down the left navigation panel and choose "Instances". Verify all the "Instances" running and terminate any "Instances" which are not required. Raise an AWS support ticket to limit the number of "Instances."</br> 
7. Click on the "Support" option at the top right corner and select the "Support Center".</br> <img src="/resources/aws/ec2/instance-limit/step7.png"/>
8. In the "Support Center" page click on the "Create Case" button.</br> <img src="/resources/aws/ec2/instance-limit/step8.png"/>
9. Select the "Service limit increase" tab and choose the "EC2 Instances" from the dropdown in "Limit Type".</br> <img src="/resources/aws/ec2/instance-limit/step9.png"/>
10. Scroll down the page and select the "Region" and "Primary Instance Type". Provide the "New limit value" as per the requirements. </br> <img src="/resources/aws/ec2/instance-limit/step10.png"/>
11. Provide a small description to your request in "Case description". </br> <img src="/resources/aws/ec2/instance-limit/step11.png"/>
12. Select  preferred contact option to the AWS Support team and click on the "Submit" button to limit request to AWS.</br> <img src="/resources/aws/ec2/instance-limit/step12.png"/>
