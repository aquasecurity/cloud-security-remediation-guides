[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Amazon EBS Public Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | Amazon EBS Public Snapshots |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that Amazon EBS volume snapshots are not shared to all AWS accounts |
| **More Info** | AWS Elastic Block Store (EBS) volume snapshots should not be not publicly shared with other AWS account to avoid data exposure |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-modifying-snapshot-permissions.html |
| **Recommended Action** | Modify the permissions of public snapshots to remove public access |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for EC2. </br> 
3. In the navigation pane, under Elastic Block Store, click on Snapshots. </br>
4. Select the snapshot to modify, and then choose Actions, Modify permissions. </br>
5. Change the snapshot's permissions. Current setting indicates the snapshot's current sharing permissions. </br>
6. To share the snapshot privately with specific AWS accounts, choose Private. Then, in the Sharing accounts section, choose Add account, and enter the 12-digit account ID (without hyphens) of the account to share with. </br>
7. Choose Save changes. </br>
8. Repeat the steps 4 - 7 for all snapshots that are shared publicly. </br>