[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Bucket Delete Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Bucket Delete Policy |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logging bucket has a policy to prevent deletion of logs without an MFA token |
| **More Info** | To provide additional security, CloudTrail logging buckets should require an MFA token to delete objects |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html#MultiFactorAuthenticationDelete |
| **Recommended Action** | Enable MFA delete on the CloudTrail bucket |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step2.png"/>
3. In the "Dashboard" panel click on "View trails" button.</br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step3.png"/>
4. Select the "trail" that needs to be verified under "Name" column.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step4.png"/>
5. Scroll down and under the "Storage location" option check the S3 bucket used to store log data.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step5.png"/>
6. Go to "Services" and search for "S3" to go into S3 buckets dashboard.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step6.png"/>
7. Select the "S3 bucket" used to store data log in CloudTrail. </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step7.png"/>
8. Enabling MFA using AWS Management Console is not supported as of now. MFA can be enabled using AWS API. Configure "AWS CLI" with your own "AWS Key Id" and "AWS Secret Key" as well as configure MFA for your root account.
9. Follow the commands to "Enable MFA".
10. To list buckets in AWS account: aws s3api list-buckets --query 'Buckets[\*].Name' </br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step10.png"/>
11. To verify if the selected "CloudTrail bucket" has object versioning enabled :  aws s3api get-bucket-versioning --bucket shukla008 </br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step11.png"/>
12. To enable "MFA Delete" and "Versioning" of the selected "CloudTrail bucket" : aws s3api put-bucket-versioning --bucket shukla008 --versioning-configuration Status=Enabled,MFADelete=Enabled --mfa 'arn:aws:iam::10260454563607:mfa/root-account-mfa-device 531098' </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step12.png"/>
13. To verify if "MFA Delete" and "Versioning" of the selected "CloudTrail bucket" is enabled. It returns output as Enabled Enabled if "MFA and Versioning" are "Enabled" : aws s3api get-bucket-versioning --bucket shukla00 </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step13.png"/>
14. To list select "CloudTrail bucket" object versions : aws s3api list-object-versions --bucket shukla008 </br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step14.png"/>
15. To examine try and delete the S3 object version without "MFA" token : aws s3api delete-object --bucket shukla008 --version-id "HBU7m.mOKZhxuXXDl5Y9c1Iu6.XWQkxu" --key demo.txt </br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-delete-policy/step15.png"/>
16. MFA Delete is enabled on selected "CloudTrail bucket".
