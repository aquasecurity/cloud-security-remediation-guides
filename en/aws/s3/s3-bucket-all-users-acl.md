[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket All Users ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket All Users ACL |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 buckets do not allow global write, delete, or read ACL permissions |
| **More Info** | S3 buckets can be configured to allow anyone, regardless of whether they are an AWS user or not, to write objects to a bucket or delete objects. This option should not be configured unless there is a strong business requirement. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/UG/EditingBucketPermissions.html |
| **Recommended Action** | Disable global all users policies on all S3 buckets and ensure both the bucket ACL is configured with least privileges. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-all-users-acl/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-logging/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step4.png"/>
5. Click on the "Permissions" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step5.png"/>
6. Check the "Acess Control List" option under "Permissions" and scroll down the configuration page and check the "Public access". If "Read bucket permissions" , "Write objects" , "List objects" and "Write bucket permissions" are set to "Yes" then the selected S3 bucket allows global write, delete, or read ACL permissions. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step6.png"/>
7. Repeat steps number 2 - 6 to verify other S3 buckets in the region. </br>
8. Select the "S3 bucket" on which global access needs to be disabled and click on the "Permissions" tab. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step8.png"/>
9. Scroll down the "Acess Control List" configuration page and under "Public access" click on the "Everyone" and uncheck the checkboxes against "Read bucket permissions" , "Write objects" , "List objects" and "Write bucket permissions". </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step10.png"/>
10. Click on the "Save" button to make the necessary changes. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step10.png"/>
11. Repeat steps number 8 - 10 to diable global write, delete, or read ACL permissions in other S3 buckets.</br>
