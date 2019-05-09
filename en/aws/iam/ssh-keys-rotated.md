[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / SSH Keys Rotated

## Quick Info

| | |
|-|-|
| **Plugin Title** | SSH Keys Rotated |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures SSH keys are not older than 180 days in order to reduce accidental exposures |
| **More Info** | SSH keys should be rotated frequently to avoid having them accidentally exposed. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_ssh-keys.html |
| **Recommended Action** | To rotate an SSH key, first create a new public-private key pair, then upload the public key to AWS and delete the old key. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/ssh-keys-rotated/step2.png"/>
3. Scroll down the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/ssh-keys-rotated/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User".</br><img src="/resources/aws/iam/ssh-keys-rotated/step4.png"/>
5. Click on the "Security Credentials" under the configuration page.</br><img src="/resources/aws/iam/ssh-keys-rotated/step5.png"/>
6. Scroll down the "Security Credentials" tab and check the "SSH keys for AWS CodeCommit" section. Check the "Uploaded" column and if any SSH key is older than 180 days than that SSH key is outdated and needs to be changed.</br><img src="/resources/aws/iam/ssh-keys-rotated/step6.png"/>
7. Repeat steps number 3 - 6 to verify any other IAM user.</br>
8. To update the SSH key scroll down the "Security Credentials" tab and check the "SSH keys for AWS CodeCommit" section. Click on "Upload SSH public key" button to upload the new SSH key.</br><img src="/resources/aws/iam/ssh-keys-rotated/step8.png"/>
9. In the "Upload SSH public key" tab upload the new SSH key and click on the "Upload SSH public key" button. </br><img src="/resources/aws/iam/ssh-keys-rotated/step9.png"/>
10. Use the new "SSH key" for AWS CodeCommit repositories and replace the older key with the new one. Make sure that the new "Access key" pair is working fine.</br>
11. To remove the older "SSH key" once you verified that the new "SSH key" is working fine click on "Security Credentials" under IAM user configuration page and select the older "SSH key ID" which needs to be removed.</br> <img src="/resources/aws/iam/ssh-keys-rotated/step11.png"/>
12. Click on the cross(×) symbol at the extreme right to remove the selected key. </br> <img src="/resources/aws/iam/ssh-keys-rotated/step12.png"/>
13. Click on "Delete" button under the "Delete SSH key" tab to delete the older "SSH Key".</br><img src="/resources/aws/iam/ssh-keys-rotated/step13.png"/>
