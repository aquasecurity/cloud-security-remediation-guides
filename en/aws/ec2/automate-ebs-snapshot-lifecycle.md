[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Automate EBS Snapshot Lifecycle

## Quick Info

| | |
|-|-|
| **Plugin Title** | Automate EBS Snapshot Lifecycle |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure DLM is used to automate EBS volume snapshots management |
| **More Info** | Amazon Data Lifecycle Manager (DLM) service enables you to manage the lifecycle of EBS volume snapshots. Using DLM helps in enforcing regular backup schedule, retaining backups, deleting outdated EBS snapshots |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/snapshot-lifecycle.html |
| **Recommended Action** | Create lifecycle policy for EBS volumes |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for EC2. </br> 
3. In the navigation pane, under Elastic Block Store, click Lifecycle Manager. </br>
4. Select a lifecycle policy from the list. Click Next Step. </br>
5. Enter the policy settings as needed. For example, add tags, and enable the policy. Click Next. </br>
6. Create the schedule as needed. </br>
7. Review and Create. </br>