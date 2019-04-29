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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br>![Step 2](/resources/aws/cloudtrail/cloudtrail-bucket-private/step2.png "Step 2 - Services")
3. In the "Dashboard" panel click on "View trails" button.</br> ![Step 3](/resources/aws/cloudtrail/cloudtrail-bucket-private/step3.png "Step 3 - Trails")
4. Select the "trail" that needs to be verified under "Name" column.</br>![Step 4](/resources/aws/cloudtrail/cloudtrail-bucket-private/step4.png "Step 4 - Name")
5. Scroll down and under the "Storage location" option check the S3 bucket used to store log data.</br>![Step 5](/resources/aws/cloudtrail/cloudtrail-bucket-private/step5.png "Step 5 - Storage")
6. Go to "Services" and search for "S3" to go into S3 buckets dashboard.</br>![Step 6](/resources/aws/cloudtrail/cloudtrail-bucket-private/step6.png "Step 6 - S3 buckets")
7. Select the "S3 bucket" used to store data log in CloudTrail and check the "Access" option. If "Access" shows "Public" than bucket is publicly accessible </br>![Step 7](/resources/aws/cloudtrail/cloudtrail-bucket-private/step7.png "Step 7 - Access")
8. Click on "Edit Public Access Settings" to configure the S3 Bucket access. </br>![Step 8](/resources/aws/cloudtrail/cloudtrail-bucket-private/step8.png "Step 8 - Public Access Settings")
9. Click on the checkboxes shown under "Manage public Access control lists (ACLs)" and "Manage public bucket policies" to make the S3 bucket private.</br>![Step 9](/resources/aws/cloudtrail/cloudtrail-bucket-private/step9.png "Step 9 - Public Access Settings")
10. Select the "S3 bucket" used by CloudTrail and click on "Permissions" tab.</br>![Step 10](/resources/aws/cloudtrail/cloudtrail-bucket-private/step10.png "Step 10 - Permissions")
11. Select the "Access Control List" from the menu and search for any group with the name "Everyone" and make sure this group has no checkboxes enabled. If this group has one or more checkboxes enabled than the selected S3 bucket is publicly accessible. </br>![Step 11](/resources/aws/cloudtrail/cloudtrail-bucket-private/step11.png "Step 11 - Access Control List")
12. Check the "Access for other AWS accounts" on the selected S3 bucket for known users.</br>![Step 12](/resources/aws/cloudtrail/cloudtrail-bucket-private/step12.png "Step 12 - Access")
13. S3 buckets access policy for all "CloudTrail buckets" have access allow only to known users now. 
