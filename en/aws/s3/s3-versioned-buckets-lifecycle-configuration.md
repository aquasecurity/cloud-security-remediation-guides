[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Versioned Buckets Lifecycle Configuration

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Versioned Buckets Lifecycle Configuration |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensure that S3 buckets having versioning enabled also have lifecycle policy configured for non-current objects. |
| **More Info** | When object versioning is enabled on a bucket, every modification/update to an object results in a new version of the object that will be stored indefinitely. Enable a lifecycle policy, so that non-current object versions are removed or transitioned in a predictable manner. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/how-to-set-lifecycle-configuration-intro.html |
| **Recommended Action** | Configure lifecycle rules for buckets which have versioning enabled. |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for S3. </br>
3. Scroll down the left navigation pane and choose "Buckets".</br> 
4. Select the "Bucket" that needs to create lifecycle rule for by clicking on its identifier(name) from the "Bucket name" column.</br>
5. Click on the "Management" tab on the top menu. </br>
6. Click on Create Lifecycle rule. </br>
7. Choose the rule scope (all bucket objects OR limit scope to specific objects using filters/ tags prefix) . </br>
8. Check Lifecycle rule actions you need to apply. </br>
9. Make sure to specify a rule for Move noncurrent versions of objects between storage classes. </br>
10. Click on the "Save" button to make the necessary changes. </br>
11. Repeat steps 4 - 10 to enable lifecycle configurations in other S3 buckets.</br>