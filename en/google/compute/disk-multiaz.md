[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk MultiAz

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk MultiAz |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** |Ensure that Compute disks have regional disk replication feature enabled for high availability.|
| **More Info** | Enabling regional disk replication will allow you to force attach a regional persistent disk to another VM instance in a different zone in the same region in case of a zonal outage. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/high-availability-regional-persistent-disk |
| **Recommended Action** | Ensure that all Google compute disks have replica zones configured. |

## Detailed Remediation Steps
You must first create the regional Persistent Disk and then attach it to an existing instance. You can't create regional Persistent Disks as boot disks because they can't be force-attached during a failover.

Create a regional Persistent Disk using the following steps:

1.  In the Google Cloud console, go to the Disks page.

    [Go to Disks](https://console.cloud.google.com/compute/disks)

2.  Select the required project.

3.  Click Create disk.

4.  Specify a Name for your disk.

5.  Select the Region and Zone. You must select the same region when you create your VM.

6.  Select the Enable regional disk replication box.

7.  Select the Replicate zone. Make a note of the zones that you select because you must attach the disk to your VM in one of those zones.

8.  Select the Disk source type.

9.  Select the Disk type.

10. Click Create to finish creating your disk.

11. After you create your regional Persistent Disk, [attach it to your instance](https://cloud.google.com/compute/docs/disks/add-persistent-disk#create_disk).
    
    When attaching a disk to a VM, if the disk is already attached to another VM, you can force-attach the disk to the VM by selecting the Force-attach disk box on the Attach existing disk page. For more information on use cases for force-attaching regional Persistent Disks, see [Regional Persistent Disk failover](https://cloud.google.com/compute/docs/disks/repd-failover).
