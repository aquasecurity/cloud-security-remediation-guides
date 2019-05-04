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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step2.png"/>
3. In the "Dashboard" panel click on "View trails" button.</br> <img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step3.png"/>
4. Select the "trail" that needs to be verified under "Name" column.</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step4.png"/>
5. Scroll down and under the "Storage location" option check for "Enable log file validation". If its status is "No" the selected trail does not support file validation.</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step5.png"/>
6. Click on the pencil icon to get into "Storage location" configuration settings. Scroll down and click on "Yes" next to "Enable log file validation" to enable the "CloudTrail" file validation to determine whether a log file was modified, deleted or unchanged after "CloudTrail" delivered it. </br> <img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step6.png"/>
7. Scroll down and click on "Save" to enable the CloudTrail log encryption.</br><img src="/resources/aws/cloudtrail/cloudtrail-file-validation/step7.png"/>
