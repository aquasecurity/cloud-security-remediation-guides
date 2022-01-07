[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / Public S3 CloudFront Origin

## Quick Info

| | |
|-|-|
| **Plugin Title** | Public S3 CloudFront Origin |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Detects the use of an S3 bucket as a CloudFront origin without an origin access identity |
| **More Info** | When S3 is used as an origin for a CloudFront bucket, the contents should be kept private and an origin access identity should allow CloudFront access. This prevents someone from bypassing the caching benefits that CloudFront provides, repeatedly loading objects directly from S3, and amassing a large access bill. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html |
| **Recommended Action** | Create an origin access identity for CloudFront, then make the contents of the S3 bucket private. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step2.png"/>
3. Select the "CloudFront Distribution" that needs to be verified.</br> <img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step3.png"/>
4. Click the "Distribution Id" to get into the "CloudFront Distribution" configuration page. </br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step4.png"/>
5. Click on the "Origins" tab and select the "Origin" which needs to be verified. Check the origin type and If it is "custom origin" then you would have to create a new origin for the same S3 Bucket. If the origin Type is "S3" then select and edit it  </br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step5.png"/>
6. Click the "Create origin" button.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step6.png"/>
7. On the "Create Origin" Page type the S3 Bucket name and select from dropdown.
8. In the S3 Bucket access select "Yes use OAI (bucket can restrict access to only CloudFront)"
9. Under the "Origin Access Identity" choose an existing Origin Access Identity else create a new OAI by clicking on "Create new OAI" button.
10. On the Origin Settings, verify the "Restrict Bucket Access".If Restrict Bucket Access is set to No then the access to the S3 bucket used as the origin is not secured.</br> <img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step7.png"/>
11. Click on the "Yes, update the bucket policy" under "Bucket Policy" so CloudFront updates bucket permissions to grant the specified origin access identity the permission to read files in your bucket.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step10.png"/>
14. Click on "Create origin" button to save the changes.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step11.png"/>
15. If you are editing an existing S3 origin then click "Edit"
16. In the S3 Bucket access select "Yes use OAI (bucket can restrict access to only CloudFront)"
9. Under the "Origin Access Identity" choose an existing Origin Access Identity else create a new OAI by clicking on "Create new OAI" button.
10. On the Origin Settings, verify the "Restrict Bucket Access".If Restrict Bucket Access is set to No then the access to the S3 bucket used as the origin is not secured.</br> <img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step7.png"/>
11. Click on the "Yes, update the bucket policy" under "Bucket Policy" so CloudFront updates bucket permissions to grant the specified origin access identity the permission to read files in your bucket.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step10.png"/>

17. Navigate to "S3 bucket dashboard" and choose the S3 bucket used to verify the "Permissions" on S3 bucket.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step12.png"/>
18. Click the "Permissons" tab and scroll to the "Block public access (bucket settings)"for the bucket.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step13.png"/>
19. Click on the "Edit" button and scroll down to "Manage public access control lists" and "Manage public bucket policies" to verify the "Permissions". Select the "Permissions" and click on "Save" to make the contents of the S3 bucket private.</br><img src="/resources/aws/cloudfront/public-s3-cloudfront-origin/step14.png"/>
20. Repeat the steps number 6 and 7 to verify origin access identity for CloudFront.</br>
