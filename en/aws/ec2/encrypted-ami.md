[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Encrypted AMI

## Quick Info

| | |
|-|-|
| **Plugin Title** | Encrypted AMI |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EBS-backed AMIs are configured to use encryption |
| **More Info** | AMIs with unencrypted data volumes can be used to launch unencrypted instances that place data at risk. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIEncryption.html |
| **Recommended Action** | Ensure all AMIs have encrypted EBS volumes. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/encrypted-ami/step2.png"/>
3. Scroll down the left navigation panel and choose "AMIs" under "Images". </br> <img src="/resources/aws/ec2/encrypted-ami/step3.png"/>
4. Select the "AMI" that needs to be verified and under "Details" tab copy the "Snapshot ID" from the "Block Devices".</br> <img src="/resources/aws/ec2/encrypted-ami/step4.png"/>
5. Scroll down the left navigation panel and choose "Snapshots" under "Elastic Block Store".</br> <img src="/resources/aws/ec2/encrypted-ami/step5.png"/>
6. Click inside the "Filter by tags and attributes or search by keyword" and from the dropdown menu choose "Snapshot ID" and paste the "Snapshot ID". </br> <img src="/resources/aws/ec2/encrypted-ami/step6.png"/>
7. Scroll down the "Description" tab and check "Encryption" value. If the "Encryption" value is set to "Not Encrypted" then the selected "AMI" is not encrypted.</br> <img src="/resources/aws/ec2/encrypted-ami/step7.png"/>
8. Repeat steps number 2 - 7 to verify other AMIs.</br>
9. Scroll down the left navigation panel and choose "AMIs" and select the "AMI" that needs to be encrypted.</br> <img src="/resources/aws/ec2/encrypted-ami/step9.png"/>
10. Click on the "Actions" button at the top and click on the "Copy AMI" option.</br> <img src="/resources/aws/ec2/encrypted-ami/step10.png"/>
11. In the "Copy AMI," dialog box select the "Destination region" from the dropdown menu and click on the "Encryption" checkbox to "Encrypt target EBS snapshots" and choose the "Master Key" from the dropdown and click on the "Copy AMI" button.</br> <img src="/resources/aws/ec2/encrypted-ami/step11.png"/>
12. Select the new "Encrypted AMI" and click on the "Launch" button to create a new EC2 instance with encrypted "EBS volume".</br> <img src="/resources/aws/ec2/encrypted-ami/step12.png"/>
13. Configure the "Instance Type", "Configure Instance Details", "Add Storage", "Security Group" as per the requirements and click on the "Review and Launch" button to create a new "EC2 Instance" backed by encrypted "EBS Volume".</br> <img src="/resources/aws/ec2/encrypted-ami/step13.png"/>
14. Repeat steps number 9 - 13 to create an "EC2 Instance" from "Encrypted AMI".</br>
