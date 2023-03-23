[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk MultiAz

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk MultiAz |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Building HA database services using regional persistent disks |
| **More Info** | You can use regional persistent disks (PDs) to build high availability (HA) services. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks/high-availability-regional-persistent-disk |
| **Recommended Action** | Build HA solutions for stateful database services. |

## Detailed Remediation Steps
This section covers high level concepts for building HA solutions for stateful database services (MySQL, Postgres, etc.) using regional persistent disks and Compute Engine.

If there are broad outages in Google Cloud, for example, if a whole region becomes unavailable, your application might become unavailable. Depending on your needs, consider [cross-regional replication techniques](https://cloud.google.com/architecture/disaster-recovery#how_to_leverage_zones_and_regions_to_achieve_reliability) for even higher availability.

Database HA configurations typically have at least two VM instances. Preferably these instances are part of one or more [managed instance groups](https://cloud.google.com/compute/docs/instance-groups/creating-groups-of-managed-instances):

-   A primary VM instance in the primary zone
-   A standby VM instance in a secondary zone

A primary VM instance has at least two persistent disks: a boot disk, and a regional persistent disk. The regional persistent disk contains database data and any other mutable data that should be preserved to another zone in case of an outage.

A standby VM instance requires a separate boot disk to be able to recover from configuration-related outages, which could result from an operating system upgrade, for example. You cannot force attach a boot disk to another VM during a failover.

The primary and standby VM instances are configured to use a load balancer with the traffic directed to the primary VM based on health check signals. This configuration is also known as a hot standby. The [disaster recovery scenario for data](https://cloud.google.com/solutions/dr-scenarios-for-data) outlines other failover configurations, which might be more appropriate for your scenario.