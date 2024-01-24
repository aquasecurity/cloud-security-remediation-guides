[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk In Use |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that there are no unused Compute disks. |
| **More Info** | Unused Compute disks should be deleted to prevent accidental exposure of data and to avoid unnecessary billing. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks |
| **Recommended Action** | Delete unused Compute disks. |

## Detailed Remediation Steps
`gcloud compute disks delete` deletes a Compute Engine disk. A disk can be deleted only if it is not attached to any virtual machine instances.</br>
<b>Example</b>
To delete the disk 'my-disk' in zone 'us-east1-a', run: </br>

`gcloud compute disks delete my-disk --zone=us-east1-a`