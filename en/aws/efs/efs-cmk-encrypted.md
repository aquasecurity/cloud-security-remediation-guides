[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EFS / EFS CMK Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | EFS CMK Encrypted |
| **Cloud** | AWS |
| **Category** | EFS |
| **Description** | Ensure EFS file systems are encrypted using Customer Master Keys (CMKs). |
| **More Info** | EFS file systems should use KMS Customer Master Keys (CMKs) instead of AWS managed keys for encryption in order to have full control over data encryption and decryption. |
| **AWS Link** | https://docs.aws.amazon.com/efs/latest/ug/encryption-at-rest.html |
| **Recommended Action** | Encryption of data at rest can only be enabled during file system creation. Encryption of data in transit is configured when mounting your file system. 1. Backup your data in not encrypted efs 2. Recreate the EFS and select 'Enable encryption of data at rest' |

## Detailed Remediation Steps
Backup your data in not encrypted efs: </br>
1. Open the Amazon Elastic File System console at https://console.aws.amazon.com/efs/. </br>
2. From Navigation pane: Click on AWS Backup. </br>
3. Click on Ceate On-demand backup. </br>
4. Select Resource type :EFS, and select the File System ID you need to create back up for. </br>
5. Fill other required info as needed then click Create backup. </br>
6. For more info on backup options follow this link: https://docs.aws.amazon.com/efs/latest/ug/awsbackup.html#restoring-backup-efs </br>

Create a new EFS and select:
1. Open the Amazon Elastic File System console at https://console.aws.amazon.com/efs/. </br>
2. Choose Create file system to open the Create file system dialog box. </br>
3. (Optional) Enter a Name for your file system. </br>
4. For Virtual Private Cloud (VPC), choose your VPC, or keep it set to your default VPC. </br>
5. Choose availability and durability. </br>
6. Click on Customize. </br>
7. Under Customize encryption settings, select KMS key. If you don't already have KMS key, click on Create an AWS KMS Key. </br>
8. See this link for more info on creating KMS keys: https://docs.aws.amazon.com/kms/latest/developerguide/create-keys.html </br>
9. Continue the steps by selecting VPC and Mount targets. </br>
10. Select the required policy options. </br>
11. Click Next to review the settings. </br>
12. Click Create. </br>. 
13. Then follow this link to restore EFS backup to the newly created EFS. https://docs.aws.amazon.com/aws-backup/latest/devguide/restoring-efs.html </br>