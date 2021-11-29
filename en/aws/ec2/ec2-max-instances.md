[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EC2 Max Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | EC2 Max Instances |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures the total number of EC2 instances does not exceed a set threshold. |
| **More Info** | The number of running EC2 instances should be carefully audited, especially in unused regions, to ensure only approved applications are consuming compute resources. Many compromised AWS accounts see large numbers of EC2 instances launched. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/monitoring_ec2.html |
| **Recommended Action** | Ensure that the number of running EC2 instances matches the expected count. If instances are launched above the threshold, investigate to ensure they are legitimate. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ec2-max-instances/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/ec2-max-instances/step3.png"/>
4. Check the total number of EC2 instances at the top left corner available in the selected AWS region. </br> <img src="/resources/aws/ec2/ec2-max-instances/step4.png"/>
5. Repeat steps number 2 - 4 to check the threshold value for other regions. If the total number of running EC2 instances provisioned in your AWS account is greater than 50, the recommended threshold was exceeded. AWS has different threshold values as well depends on the region. Raise an AWS support ticket to limit the number of instances as per the requirements. </br>
6. Scroll down the left navigation panel and choose "Instances". Verify all the "Instances" running and terminate any "Instances" which are not required. 
7. Choose the "EC2 Instances" which are not required from the "Instances" configuration page. </br> <img src="/resources/aws/ec2/ec2-max-instances/step7.png"/>
8. Click on the "Instance State" button at the top panel and click on "Stop instance" to stop the selected "EC2 Instance".</br> <img src="/resources/aws/ec2/ec2-max-instances/step8.png"/>
9. Click on the "Instance state" button at the top panel and click on "Terminate Instance"  to terminate the selected "EC2 Instance". </br> <img src="/resources/aws/ec2/ec2-max-instances/step9.png"/> 
10. On the "Terminate Instance" dialog box click on the "Terminate" button.</br> <img src="/resources/aws/ec2/ec2-max-instances/step10.png"/>
11. Repeat steps number 6 - 10 to remove the "EC2 Instances" which are not required. </br>
