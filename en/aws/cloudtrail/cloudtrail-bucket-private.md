[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Bucket Private

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Bucket Private |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logging bucket is not publicly accessible |
| **More Info** | CloudTrail buckets contain large amounts of sensitive account data and should only be accessible by logged in users. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html |
| **Recommended Action** | Set the S3 bucket access policy for all CloudTrail buckets to only allow known users to access its files. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step2.png"/>
3. In the "Dashboard" panel click on the desired trail from the list under "Trails" to get to its configuration page.</br> <img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step3.png"/>
4. Click on "Edit" under "General details".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step4.png"/>
5. Scroll down and under the "Storage location" option check the S3 bucket used to store log data.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step5.png"/>
6. Go to "Services" and search for "S3" to go into S3 buckets dashboard.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step6.png"/>
7. Select the "S3 bucket" used to store data log in CloudTrail and check the "Access" option. If "Access" shows "Objects can be public" than bucket is publicly accessible </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step7.png"/>
8. Click on the Bucket name to get into its configuration page. </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step8.png"/>
9. Click on the "Permissions" tab and scroll down to "Block public access (bucket settings)" and click "Edit".</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step9.png"/>
10. Select the checkbox "Block all public access" shown under "Block public access (bucket settings)" to make the S3 bucket private.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step10.png"/>
11. Click on "save changes" to save the settings.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step11.png"/>
12. On the permissions tab scroll down to "Access control list (ACL)" to check the access for other AWS accounts on the selected S3 bucket for known users. Click "Edit" to add permissions for accounts as desired.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step12.png"/>
13. On the "Edit access control list (ACL)" page click on "Add grantee" button to grant access to other AWS accounts as desired.</br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step13.png"/>
14. Under "Access for other AWS accounts" paste the Canonical ID of the desired AWS account and check desired permissions. Review and click "Save changes". </br><img src="/resources/aws/cloudtrail/cloudtrail-bucket-private/step14.png"/>
15. Repeat steps 4 to 14 for all other Cloudtrail trails.
