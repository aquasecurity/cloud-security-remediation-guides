[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Lifecycle Configuration

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Lifecycle Configuration |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures that S3 buckets have lifecycle configuration enabled to automatically transition S3 bucket objects. |
| **More Info** | S3 bucket should have lifecycle configuration enabled to automatically downgrade the storage class for your objects. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/dev/how-to-set-lifecycle-configuration-intro.html |
| **Recommended Action** | Update S3 bucket and create lifecycle rule configuration. |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for S3. </br>
3. Scroll down the left navigation pane and choose "Buckets".</br> 
4. Select the "Bucket" that needs to add policy to and click on its identifier(name) from the "Bucket name" column.</br>
5. Click on the "Management" tab on the top menu. </br>
6. Click on Create Lifecycle rule. </br>
7. Choose the rule scope (all bucket objects OR limit scope to specific objects using filters/ tags prefix) . </br>
8. Check Lifecycle rule actions you need to apply. </br>
9. Click on the "Save" button to make the necessary changes. </br>
10. Repeat steps number 4 - 9 to enable lifecycle configurations in other S3 buckets.</br>