[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket MFA Delete Status

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket MFA Delete Status |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures MFA delete is enabled on S3 buckets. |
| **More Info** | Adding MFA delete adds another layer of security while changing the version state in the event of security credentials being compromised or unauthorized access being granted. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/userguide/MultiFactorAuthenticationDelete.html |
| **Recommended Action** | Enable MFA Delete on S3 buckets. |

## Detailed Remediation Steps
**Note**
you cannot enable MFA Delete using the AWS Management Console. You must use the AWS Command Line Interface (AWS CLI) or the API.

**Using the AWS CLI**
The following example enables S3 Versioning and multi-factor authentication (MFA) delete on a bucket.

```
aws s3api put-bucket-versioning --bucket amzn-s3-demo-bucket1 --versioning-configuration Status=Enabled,MFADelete=Enabled --mfa "SERIAL 123456"			
``` 	
The serial number is the number that uniquely identifies the MFA device. For physical MFA devices, this is the unique serial number that's provided with the device. For virtual MFA devices, the serial number is the device ARN.

To enable MFA using the REST API see [PutBucketVersioning Amazon Simple Storage Service API Reference](https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketVersioning.html).

**Note**
MFA delete requires additional authentication for either of the following operations:
1. Changing the versioning state of your bucket.
2. Permanently deleting an object version.

[You cannot use MFA delete with lifecycle configurations](https://docs.aws.amazon.com/AmazonS3/latest/userguide/lifecycle-and-other-bucket-config.html).
