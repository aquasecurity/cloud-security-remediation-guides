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
For synchronous and asynchronous application replication:

-   Use two instances of the database and VM. In this case the following items determine the total cost:

    -   VM instance costs
    -   Persistent disk costs
    -   Costs of maintaining application replication
-   Use a single VM with regional persistent disks. To achieve high availability with a regional persistent disk, use the same VM instance and persistent disk components, but also include a regional persistent disk. Regional persistent disks are double the cost per byte compared to zonal persistent disks because they are replicated in two zones.

    However, using regional persistent disks might reduce your maintenance cost because the data is automatically replicated to two replicas without the requirement of maintaining application replication.

-   Do not start the second VM until failover is required. You can reduce host costs even more by starting the back-up VM only on demand during failover rather than maintaining the VM as a hot standby.
