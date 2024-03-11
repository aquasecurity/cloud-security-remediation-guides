[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database Instance Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database Instance Encrypted |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensure that your AWS Neptune database instances are encrypted with KMS Customer Master Keys (CMKs) instead of AWS managed-keys |
| **More Info** | Neptune encrypted instances provide an additional layer of data protection by helping to secure your data from unauthorized access to the underlying storage. You can use Neptune encryption to increase data protection of your applications that are deployed in the cloud. You can also use it to fulfill compliance requirements for data-at-rest encryption. |
| **AWS Link** | https://docs.aws.amazon.com/neptune/latest/userguide/encrypt.html |
| **Recommended Action** | Encrypt Neptune database with desired encryption level |

## Detailed Remediation Steps
1. You cannot convert an unencrypted DB instance to an encrypted one. You can only enable encryption for a DB instance when you create it. </br>
2. To enable encryption for a new Neptune DB instance, choose Yes in the Enable encryption section on the Neptune console. For information about creating a Neptune DB instance, see https://docs.aws.amazon.com/neptune/latest/userguide/get-started-create-cluster.html </br>
3. However, you can restore an unencrypted DB cluster snapshot to an encrypted DB cluster. To do this, specify a KMS encryption key when you restore from the unencrypted DB cluster snapshot. </br>
4. Also, DB instances that are encrypted can't be modified to disable encryption. </br>
5. You can't have an encrypted Read Replica of an unencrypted DB instance, or an unencrypted Read Replica of an encrypted DB instance. </br>
6. Encrypted Read Replicas must be encrypted with the same key as the source DB instance. </br>