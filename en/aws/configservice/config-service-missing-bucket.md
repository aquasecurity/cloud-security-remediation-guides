[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ConfigService / Config Service Missing Bucket

## Quick Info

| | |
|-|-|
| **Plugin Title** | Config Service Missing Bucket |
| **Cloud** | AWS |
| **Category** | ConfigService |
| **Description** | Ensure that Amazon Config service is pointing an S3 bucket that is active in your account in order to save configuration information. |
| **More Info** | Amazon Config tracks changes within the configuration of your AWS resources and it regularly sends updated configuration details to an S3 bucket that you specify. When AWS Config is not referencing an active S3 bucket, the service is unable to send the recorded information to the designated bucket, therefore you lose the ability to audit later the configuration changes made within your AWS account.  |
| **AWS Link** | https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-policy.html |
| **Recommended Action** | Ensure that Amazon Config service is referencing an active S3 bucket in order to save configuration information. |