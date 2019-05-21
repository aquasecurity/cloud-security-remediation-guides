[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Encrypted Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Encrypted Snapshots |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EBS snapshots are encrypted at rest |
| **More Info** | EBS snapshots should have at-rest encryption enabled through AWS using KMS. If the volume was not encrypted and a snapshot was taken the snapshot will be unencrypted. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html#encryption-support |
| **Recommended Action** | Configure volume encryption and delete unencrypted EBS snapshots. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step2.png"/>
3. Scroll down the left navigation panel and choose "Snapshots". </br>  <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step3.png"/>
4. Select the "Snapshot" that needs to be verified and click on its name from the "Name" column.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step4.png"/>
5. Scroll down the page and under "Description" check for "Encrypted". If the "Encrypted" option is showing "Not Encrypted" then the selected the "EBS Snapshot" is not encrypted.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step5.png"/>
6. Repeat the steps number 2 - 5 to check other "EBS Snapshot" in the AWS region.</br>
7. Select the unencrypted "EBS Snapshot" that needs to be encrypted and click on the "Actions" button at the top panel and click on the "Copy" option.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step7.png"/>
8. In the "Copy Snapshot" dialog box select the box "Encrypt this snapshot" next to "Encryption" and choose the "Master key" from the dropdown menu.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step8.png"/>
9. Click on the "Copy" button to copy the selected "EBS Snapshot". </br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step9.png"/>
10. Select the new EBS snapshot and click on the "Actions" button at the top panel and click on the "Create Volume" option.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step10.png"/>
11. In the "Create Volume" dialog box verify the "Encryption" option is enabled.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step11.png"/>
12. Click on the "Create Volume" button to create the new "EBS Encrypted Volume".</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step12.png"/>
13. Scroll down the left navigation panel and click on the "Volumes".</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step13.png"/>
14. Select the volume that is not encrypted and click on the "Action" button at the top and click on the "Detach Volume".</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step14.png"/>
15. In the "Detach Volume" dialog box click on the "Yes,Detach" button. </br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step15.png"/>
16. Select the newly encrypted EBS volume and click on the "Action" button at the top and click on the "Attach Volume".</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step16.png"/>
17. In the "Attach Volume" dialog box select the EC2 instance and device name for the attachment.</br> <img src="/resources/aws/ec2/ebs-encrypted-snapshots/step17.png"/> 
18. Repeat steps number 7 - 17 to ensure "EBS snapshots" are encrypted at rest.
