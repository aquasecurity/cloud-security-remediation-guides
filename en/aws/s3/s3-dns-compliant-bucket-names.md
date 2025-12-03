[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 DNS Compliant Bucket Names

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 DNS Compliant Bucket Names |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures that S3 buckets have DNS complaint bucket names. |
| **More Info** | S3 bucket names must be DNS-compliant and not contain period "." to enable S3 Transfer Acceleration and to use buckets over SSL. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html |
| **Recommended Action** | Recreate S3 bucket to use "-" instead of "." in S3 bucket names. |