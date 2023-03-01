[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk Old Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk Old Snapshots |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Compute disk snapshots are deleted after defined time period. |
| **More Info** | To optimize storage costs, make sure that there are no old disk snapshots in your GCP project. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/create-snapshots |
| **Recommended Action** | Ensure that there are no snapshots older than specified number of days. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. In the left navigation panel choose "Compute Engine" and then select the "Snapshots" option.
3. Select the snapshots that are older than the specified number of days.
4. At the top of the Snapshots page, click Delete.