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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for S3. </br> <img src="/resources/aws/s3/s3-bucket-all-users-acl/step2.png"/>
3. Scroll down the left navigation panel and choose "Buckets".</br> <img src="/resources/aws/s3/s3-bucket-all-users-acl/step3.png"/>
4. Select the "Bucket" that needs to be verified and click on its identifier(name) from the "Bucket name" column.</br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step4.png"/>
5. Click on the "Permissions" tab on the top menu. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step5.png"/>
6. Check the "Acess Control List" option under "Permissions" and scroll down the configuration page and check the "Block public access (bucket settings). If 
its status is "Off" then  public access to your S3 bucket and objects is open. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step6.png"/>
7. Scroll down to "Access control list (ACL)" and verify if the bucket allows "Everyone (public access)".</br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step7.png"/>
8. If public List, Read or Write is Enabled in step 6 or 7 then disable by clicking "Edit" in "Block public access (bucket settings)" and select "Block all public access" and click "Save changes" button. </br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step8.png"/>
9. In the "Edit Block public access (bucket settings)" confirmation box type "confirm" in the text box and click "Confirm" button.</br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step9.png"/>
10. Scroll down to "Access control list (ACL)" and click "Edit". On the "Edit access control list (ACL)" page uncheck all checkboxes other than "Bucket owner (your AWS account)" and click on "Save changes" button.</br><img src="/resources/aws/s3/s3-bucket-all-users-acl/step10.png"/>
11. Repeat steps number 4 - 10 to diable global write, delete, or read ACL permissions in other S3 buckets.</br>
