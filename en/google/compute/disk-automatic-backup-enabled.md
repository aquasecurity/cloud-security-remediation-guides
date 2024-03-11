[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk Automatic Backup Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk Automatic Backup Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Google Compute disks have scheduled snapshots configured. |
| **More Info** | Having scheduled snapshots configured for your disks will periodically backup data from your persistent disks. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/scheduled-snapshots |
| **Recommended Action** | Ensure that all compute disks have a snapshot schedule attached. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "Disks" option.
3. Click the name of the disk to which you want to attach a snapshot schedule. This opens the disk details page.
4. At the top of the disk details page, click Edit.
5. Use the Snapshot schedule drop-down menu to add the schedule to the disk. Or create a new schedule.
6. If you created a new schedule, click Create.
7. Click Save to complete the task.

**These configuration changes may incur additional costs**