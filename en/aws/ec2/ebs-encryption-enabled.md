[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Encryption Enabled |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EBS volumes are encrypted at rest |
| **More Info** | EBS volumes should have at-rest encryption enabled through AWS using KMS. If the volume is used for a root volume, the instance must be launched from an AMI that has been encrypted as well. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html |
| **Recommended Action** | Enable encryption for EBS volumes. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Volumes". </br>  <img src="/resources/aws/ec2/ebs-encryption-enabled/step3.png"/>
4. Select the "Volume" that needs to be verified and click on its name from the "Name" column.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step4.png"/>
5. Scroll down the page and under "Description" check for "Encrypted". If the "Encrypted" option is showing "Not Encrypted" then the selected the "EBS Volume" is not encrypted.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step5.png"/>
6. Repeat the steps number 2 - 5 to check other "EBS Snapshot" in the AWS region.</br>
7. Select the unencrypted "EBS Volume" that needs to be encrypted and click on the "Actions" button at the top panel and click on the "Create Snapshot" option.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step7.png"/>
8. Provide the description of the new snapshot in the "Create Snapshot" dialog box and click on the "Create Snapshot" button.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step8.png"/>
9. Scroll down the left navigation panel and choose "Snapshots".</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step9.png"/>
10. Select the new "EBS Snapshot" created and click on the "Actions" button at the top panel and click on the "Copy" option.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step10.png"/>
11. In the "Copy Snapshot" dialog box select the box "Encrypt this snapshot" next to "Encryption" and choose the "Master key" from the dropdown menu.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step11.png"/>
12. Click on the "Copy" button to copy the selected "EBS Snapshot". </br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step12.png"/>
13. Select the new EBS snapshot and click on the "Actions" button at the top panel and click on the "Create Volume" option.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step13.png"/>
14. In the "Create Volume" dialog box verify the "Encryption" option is enabled.</br><img src="/resources/aws/ec2/ebs-encryption-enabled/step14.png"/>
15. Click on the "Create Volume" button to create the new "EBS Encrypted Volume".</br><img src="/resources/aws/ec2/ebs-encryption-enabled/step15.png"/>
16. Scroll down the left navigation panel and click on the "Volumes".</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step16.png"/>
17. Select the volume that is not encrypted and click on the "Action" button at the top and click on the "Detach Volume".</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step17.png"/>
18. In the "Detach Volume" dialog box click on the "Yes,Detach" button. </br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step18.png"/>
19. Select the newly encrypted EBS volume and click on the "Action" button at the top and click on the "Attach Volume".</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step19.png"/>
20. In the "Attach Volume" dialog box select the EC2 instance and device name for the attachment.</br> <img src="/resources/aws/ec2/ebs-encryption-enabled/step20.png"/>
21. Repeat steps number 7 - 20 to ensure "EBS Volume" encryption is enabled.</br>
