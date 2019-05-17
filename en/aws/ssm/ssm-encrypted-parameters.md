[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SSM / SSM Encrypted Parameters

## Quick Info

| | |
|-|-|
| **Plugin Title** | SSM Encrypted Parameters |
| **Cloud** | AWS |
| **Category** | SSM |
| **Description** | Ensures SSM Parameters are encrypted |
| **More Info** | SSM Parameters should be encrypted. This allows their values to be used by approved systems, while restricting access to other users of the account. |
| **AWS Link** | https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-paramstore-about.html#sysman-paramstore-securestring |
| **Recommended Action** | Recreate unencrypted SSM Parameters with Type set to SecureString. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for SSM. </br> <img src="/resources/aws/ssm/ssm-encrypted-parameters/step2.png"/>
3. Scroll down the left navigation panel and choose "Parameters" under "Shared Resources". </br> <img src="/resources/aws/ssm/ssm-encrypted-parameters/step3.png"/>
4. Select the "SSM Parameter" that needs to be verified and click on its name from the "Name" column.</br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step4.png"/>
5. Scroll down the "Parameter Store" configuration page and if the selected "Parameter" holds important information such as passwords, security tokens as values under "Value" attribute and "Type" are showing as "String" then the selected SSM parameter is not encrypted. </br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SSM Parameters". </br>
7. Select the unencrypted "SSM Parameter" that needs to be re-created and click on its name from "Name" column and copy the values set for the "Name", "Description" and "Value attributes" in another location.</br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step7.png"/>
8. Click on the Parameter Store and delete the unencrypted "SSM Parameter" by clicking on "Delete" button at the top panel. </br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step8.png"/>
9. Click on the "Create parameter" button at the top panel. </br> <img src="/resources/aws/ssm/ssm-encrypted-parameters/step9.png"/>
10. Copy the value set for the "Name", "Description" and "Value attributes" from the location where we copied earlier.</br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step10.png"/>
11. Choose "SecureString" under "Type" and choose whether to use "KMS key" from current account or from another account and choose the "KMS Key ID" from dropdown menu accordingly and provide the "Value" which needs to be encrypted.</br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step11.png"/>
12. Scroll down and click on the "Create parameter" button. </br><img src="/resources/aws/ssm/ssm-encrypted-parameters/step12.png"/>
13. Repeat the steps number 6 - 12 to recreate unencrypted "SSM Parameters" with "Type" set to "SecureString".</br>
