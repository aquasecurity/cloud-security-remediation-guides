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
1.Log into the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> ![Step 2](/resources/aws/cloudfront/public-s3-cloudfront-origin/step2.png "Step 2 - Services")
3. Select the "CloudFront Distribution" that needs to be verified.</br> ![Step 3](/resources/aws/cloudfront/public-s3-cloudfront-origin/step3.png "Step 3 - CloudFront Distribution")
4. Click the "Distribution Settings" button from menu to get into the "CloudFront Distribution" configuration page. </br>![Step 4](/resources/aws/cloudfront/public-s3-cloudfront-origin/step4.png "Step 4 - Distribution Settings")
5. Click the "Origins and Origin Groups" button from the top menu to get into the "Origins" configuration page and select the "Origin" which needs to be verified.</br>![Step 5](/resources/aws/cloudfront/public-s3-cloudfront-origin/step5.png "Step 5 - Origin and Origin Groups")
6. Click the "Edit" button from the "Origins" tab on the menu.</br>![Step 6](/resources/aws/cloudfront/public-s3-cloudfront-origin/step6.png "Step 6 - Edit")
7. On the Origin Settings, verify the "Restrict Bucket Access".If Restrict Bucket Access is set to No then the access to the S3 bucket used as the origin is not secured.</br> ![Step 7](/resources/aws/cloudfront/public-s3-cloudfront-origin/step7.png "Step 7 - Restrict Bucket Access")
8. On the "Restrict Bucket Access" choose "Yes" so it requires that users always access your Amazon S3 content using CloudFront URLs, not Amazon S3 URLs.</br>![Step 8](/resources/aws/cloudfront/public-s3-cloudfront-origin/step8.png "Step 8 - Restrict Bucket Access")
9. On the "Origin Access Identity" choose "Create a New Identity" and if already have an origin access identity, click use an "Existing Identity". Enter a comment that can be used to identify the new origin access identity.</br>![Step 9](/resources/aws/cloudfront/public-s3-cloudfront-origin/step9.png "Step 9 - Origin Access Identity")
10. Click on the "Yes, Update Bucket Policy" on "Grant Read Permissions on Bucket" so CloudFront updates bucket permissions to grant the specified origin access identity the permission to read files in your bucket.</br>![Step 10](/resources/aws/cloudfront/public-s3-cloudfront-origin/step10.png "Step 10 - Bucket Policy")
11. Click on "Yes,Edit" button to save the changes.</br>![Step 11](/resources/aws/cloudfront/public-s3-cloudfront-origin/step11.png "Step 11 - Edit")
12. Navigate to "S3 bucket dashboard" and choose the S3 bucket used to verify the "Permissions" on S3 bucket.</br>![Step 12](/resources/aws/cloudfront/public-s3-cloudfront-origin/step12.png "Step 12 - S3 bucket")
13. Click the "Permissons" tab from menu to get into the "Public access settings" for the bucket.</br>![Step 13](/resources/aws/cloudfront/public-s3-cloudfront-origin/step13.png "Step 13 - Permissions")
14. Click on the "Edit" button and scroll down to "Manage public access control lists" and "Manage public bucket policies" to verify the "Permissions". Select the "Permissions" and click on "Save" to make the contents of the S3 bucket private.</br>![Step 14](/resources/aws/cloudfront/public-s3-cloudfront-origin/step14.png "Step 14 - Bucket Policies")
15. Repeat the steps number 6 and 7 to verify origin access identity for CloudFront.</br>

