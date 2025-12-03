[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Volumes Too Old Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Volumes Too Old Snapshots |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that EBS volume snapshots are deleted after defined time period |
| **More Info** | EBS volume snapshots older than indicated should be deleted after defined time period for cost optimization |
| **AWS Link** | https://docs.amazonaws.cn/en_us/AWSEC2/latest/UserGuide/ebs-deleting-snapshot.html |
| **Recommended Action** | Delete the EBS snapshots past their defined expiration date, the default expiration time is 30 days |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for EC2. </br> 
3. In the navigation pane, under Elastic Block Store, click on Snapshots. </br>
4. Select the snapshot to delete, and then choose Actions, Delete snapshot. </br>
5. Choose Delete. </br>