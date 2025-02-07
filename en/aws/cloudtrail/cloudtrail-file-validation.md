[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail File Validation

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail File Validation |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail file validation is enabled for all regions within an account |
| **More Info** | CloudTrail file validation is essentially a hash of the file which can be used to ensure its integrity in the case of an account compromise. |
| **AWS Link** | http://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-log-file-validation-enabling.html |
| **Recommended Action** | Enable CloudTrail file validation for all regions |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step2.png"/>
3. In the "Dashboard" panel click on the desired trail from the list under "Trails" to get to its configuration page.</br> <img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step3.png"/>
4. Click on "Edit" under "General details". </br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step4.png"/>
5. Scroll down and under the "Additional settings" option check for "Log file validation". If its status is not selected as "Enabled" then the selected trail does not support file validation.</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step5.png"/>
6. Click on the checkbox under "Log file validation" to change its status to "Enabled" so that the "CloudTrail" file validation to determine whether a log file was modified, deleted or unchanged after "CloudTrail" delivered is enabled. </br> <img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step6.png"/>
7. Scroll down and click on "Save changes" to enable the CloudTrail log encryption.</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step7.png"/>
