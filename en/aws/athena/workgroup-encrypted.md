[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Athena / Workgroup Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Workgroup Encrypted |
| **Cloud** | AWS |
| **Category** | Athena |
| **Description** | Ensures Athena workgroups are configured to encrypt all data at rest. |
| **More Info** | Athena workgroups support full server-side encryption for all data at rest which should be enabled. |
| **AWS Link** | https://docs.aws.amazon.com/athena/latest/ug/encryption.html |
| **Recommended Action** | Enable encryption at rest for all Athena workgroups. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for Athena. </br> <img src="/resources/aws/athena/workgroup-encrypted/step2.png"/>
3. On the "Athena" dashboard, choose the "Settings" option at the top right console.</br> <img src="/resources/aws/athena/workgroup-encrypted/step3.png"/>
4. On the "Settings" tab, for Query result location, enter a custom value or leave the default. This is the Amazon S3 staging directory where query results are stored.</br> <img src="/resources/aws/athena/workgroup-encrypted/step4.png"/>
5. Go through "Encrypt query results" option and check whether Athena workgroups are configured to encrypt all data at rest.</br> <img src="/resources/aws/athena/workgroup-encrypted/step5.png"/>
6. Repeat steps number 2 - 5 to check other Athena Workgroups in the account.</br>
7. Navigate to the Athena console using the link https://console.aws.amazon.com/athena/ .</br>
8. On the "Athena Console", click on the "Settings" option at the top right and in the "Settings" tab look for "Encrypt Query results" and click on the checkbox. </br> <img src="/resources/aws/athena/workgroup-encrypted/step8.png"/>
9. For Encryption type, choose CSE-KMS, SSE-KMS, or SSE-S3.</br> <img src="/resources/aws/athena/workgroup-encrypted/step9.png"/>
10. If you chose SSE-KMS or CSE-KMS, specify the Encryption key.</br> <img src="/resources/aws/athena/workgroup-encrypted/step10.png"/>
11. If your account has access to an existing AWS KMS customer managed key (CMK), choose its alias or choose Enter a KMS key ARN and then enter an ARN.</br>
12. If your account does not have access to an existing AWS KMS customer managed key (CMK), choose Create KMS key.</br> <img src="/resources/aws/athena/workgroup-encrypted/step12.png"/>
13. Click on the "Save" button to make the changes.</br> <img src="/resources/aws/athena/workgroup-encrypted/step13.png"/>
14. Repeat steps number 7 - 13 to enable encryption at rest for all Athena workgroups.</br>



