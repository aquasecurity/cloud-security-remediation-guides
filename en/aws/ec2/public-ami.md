[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Public AMI

## Quick Info

| | |
|-|-|
| **Plugin Title** | Public AMI |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Checks for publicly shared AMIs |
| **More Info** | Accidentally sharing AMIs allows any AWS user to launch an EC2 instance using the image as a base. This can potentially expose sensitive information stored on the host. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/sharingamis-intro.html |
| **Recommended Action** | Convert the public AMI a private image. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/public-ami/step2.png"/>
3. Scroll down the left navigation panel and choose "AMIs" under "Images".</br> <img src="/resources/aws/ec2/public-ami/step3.png"/>
4. Select the "AMI" that needs to be verified. </br> <img src="/resources/aws/ec2/public-ami/step4.png"/>
5. Scroll down the page and select the "Permissions" tab from the dashboard bottom panel and check the AMI permission. If the selected AMI is publicly accessible it will show "This image is currently Public". This can potentially expose sensitive information stored on the host.</br> <img src="/resources/aws/ec2/public-ami/step5.png"/>
6. Repeat steps number 2 - 6 to verify ohter "AMIs" permissions in the region.</br>
7. Navigate to "AMIs" under "Images" and select the "AMI" that needs to modify to restrict the publicly shared image to private image.</br> <img src="/resources/aws/ec2/public-ami/step7.png"/>
8. Click on the "Permissions" tab from the dashboard bottom panel and click on the "Edit" button.</br> <img src="/resources/aws/ec2/public-ami/step8.png"/>
9. In the "Modify Image Permissions" choose "Private" and click on the "Save" button to make the necessary changes.</br> <img src="/resources/aws/ec2/public-ami/step9.png"/>
10. Repeat steps number 7 - 9 to change "Public AMI" to the "Private AMI" in the selected AWS region.</br>
