[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Persistent Disk Auto Delete

## Quick Info

| | |
|-|-|
| **Plugin Title** | Persistent Disk Auto Delete |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Automatically delete read/write zonal persistent disks when the associated VM instance is deleted |
| **More Info** | This behavior is controlled by the autoDelete property on the VM instance for a given attached zonal persistent disk and can be updated at any time. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks |
| **Recommended Action** | Set the auto-delete state of a zonal persistent disk. |

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the VM instances page.

    [Go to VM instances](https://console.cloud.google.com/compute/instances)

2.  Select the instance that has the disks associated with it.

3.  Click the instance name. The VM instance details page appears.

4.  Click Edit.

5.  In the Storage section, under the heading Additional disks, click the pencil icon mode_edit to change the disk's Deletion Rule.

6.  Click Save to update your instance.