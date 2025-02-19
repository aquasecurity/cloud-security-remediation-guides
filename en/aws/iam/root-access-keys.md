[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root Access Keys

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root Access Keys |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the root account is not using access keys |
| **More Info** | The root account should avoid using access keys. Since the root account has full permissions across the entire account, creating access keys for it only increases the chance that they are compromised. Instead, create IAM users with predefined roles. |
| **AWS Link** | http://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html |
| **Recommended Action** | Remove access keys for the root account and setup IAM users with limited permissions instead |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Click on the AWS account name at the top on AWS management console and click on the "Security Credentials" from the menu.</br><img src="/resources/aws/iam/root-access-keys/step2.png"/>
3. On the "My security credentials" page scroll down to "Access keys for CLI, SDK, & API access". Check the "Status" column under "Access Keys" and see if there are any "Active" keys in the root account. If there are one or more active keys than AWS account might get compromised against unauthorized access.</br><img src="/resources/aws/iam/root-access-keys/step3.png"/>
4. Select the "Access Key" which is "Active" under "Status" column. Click on the "Delete" option at the extreme right to delete the selected key.</br><img src="/resources/aws/iam/root-access-keys/step4.png"/>
5. On the "Delete Access Key" pop up click on "Deactivate" button to deactivate the selected key.</br><img src="/resources/aws/iam/root-access-keys/step5.png"/>
6. To confirm deletion enter the access key ID in the text input field and click on "Delete" button. </br><img src="/resources/aws/iam/root-access-keys/step6.png"/>
7. Repeat steps number 2 and 6 for other AWS accounts.</br>
