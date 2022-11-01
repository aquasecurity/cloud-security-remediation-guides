[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Backup Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Backup Enabled |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Checks whether EBS Backup is enabled |
| **More Info** | EBS volumes should have backups in the form of snapshots |
| **AWS Link** | https://docs.aws.amazon.com/prescriptive-guidance/latest/backup-recovery/new-ebs-volume-backups.html |
| **Recommended Action** | Ensure that each EBS volumes contain at least a backup in the form of a snapshot. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br>
3. On Amazon EC2 console, on the Elastic Block Store Volumes page, select the volume that you want to back up. </br>
4. Then on the Actions menu, choose Create Snapshot. </br>
5. You can search for volumes that are attached to a specific instance by entering the instance ID in the filter box. </br>
6. Enter a description and add the appropriate tags. </br>
7. Add a Name tag to make it easier to find the volume later. </br> 
8. Add any other appropriate tags based on your tagging strategy. </br> 
9. Repeat steps 3 - 8 for each EBS volume that does not have a snapshot. </br>