[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Access Keys Rotated

## Quick Info

| | |
|-|-|
| **Plugin Title** | Access Keys Rotated |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures access keys are not older than 180 days in order to reduce accidental exposures |
| **More Info** | Access keys should be rotated frequently to avoid having them accidentally exposed. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | To rotate an access key, first create a new key, replace the key and secret throughout your app or scripts, then set the previous key to disabled. Once you ensure that no services are broken, then fully delete the old key. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/access-keys-rotated/step2.png"/>
3. Scroll down the left navigation panel and choose "Users" under "Access Management". </br><img src="/resources/aws/iam/access-keys-rotated/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User" and go to its configuration page.
</br><img src="/resources/aws/iam/access-keys-rotated/step4.png"/>
5. Scroll down and under "Security Credentials" check the "Last used" cloumn in "Access keys" to determine the last date of "Access Key" used.Any key above 180 days which is "Active" is old and expired and needs to be updated to reduce accidental exposures.</br><img src="/resources/aws/iam/access-keys-rotated/step5.png"/>
6. Click on "Create access key" to create a new key. You can have a maximum of two access keys (active or inactive) at a time.</br><img src="/resources/aws/iam/access-keys-rotated/step6.png"/>
7. Click on the "Download .csv file" to download the new "Secret Access Key" and "Access Key ID" for newly created "Access key".</br><img src="/resources/aws/iam/access-keys-rotated/step7.png"/>
8. Use the new "Access Key" for application(s) code and replace the older key with the new one. Make sure that new "Access key" pair is working fine.</br>
9. To remove the older "Access Key" once you verified that the new "Access Key" is working fine click on the "Security Credentials" under IAM user configuration page and select the older "Access Key ID" which needs to be removed. Click on the cross(×) symbol at the extreme right to remove the selected key.</br><img src="/resources/aws/iam/access-keys-rotated/step9.png"/>
10. Click on "Deactivate" button in the delete confirmation popup box.</br><img src="/resources/aws/iam/access-keys-rotated/step10.png"/>
11. Enter "Access key Id" in the text box and press the "Delete" button to delete the extra "Access Key".</br><img src="/resources/aws/iam/access-keys-rotated/step11.png"/>
12. Repeat steps number 4 - 11 to check the "Access Keys" for all other IAM users.

