[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Application Consistent Snapshots

## Quick Info

| | |
|-|-|
| **Plugin Title** | Application Consistent Snapshots |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that application consistent snapshots feature is enabled for snapshot schedules. |
| **More Info** | Application consistent snapshots are more reliable because they are created after making sure that current operations are temporarily ceased and any data in memory is flushed to disk. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/snapshot-best-practices#prepare_for_consistency |
| **Recommended Action** | Ensure that all disk snapshot schedules are application consistent. |

## Detailed Remediation Steps
### Preparing for consistent snapshots
If you create a snapshot of your persistent disk or Hyperdisk while your application is running, the snapshot might not capture pending writes that are in transit from memory to disk. Because of these inconsistencies, the snapshot might not reflect the exact state of your application at the time you captured the snapshot. In this scenario, the snapshot is considered crash consistent because it captures the state of the application as if the machine crashed at the time the snapshot was taken.

Optionally, you can pause the application, so that all application transactions complete and the system can flush all pending writes from memory to disk before the snapshot is captured. In this scenario, the snapshot is considered application consistent.

### Creating Application Consisten Snapshots
-   Windows Server users: For persistent disks that are attached to Windows Server instances, use [VSS snapshots](https://cloud.google.com/compute/docs/instances/windows/creating-windows-persistent-disk-snapshot).
-   Linux users: To achieve application consistency for snapshots of disks attached to Linux instances, create pre and post snapshot shell scripts to prepare your system for application consistency. Then create a snapshot with the `guest-flush` option enabled. This runs the pre and post scripts before and after the snapshot is captured. For instructions, see [Creating Linux application consistent snapshots](https://cloud.google.com/compute/docs/disks/creating-linux-application-consistent-pd-snapshots).
