[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Object Store / Bucket Public Access Type

## Quick Info

| | |
|-|-|
| **Plugin Title** | Bucket Public Access Type |
| **Cloud** | ORACLE |
| **Category** | Object Store |
| **Description** | Ensures object store buckets do not allow global write, delete, or read permissions |
| **More Info** | Object store buckets can be configured to allow anyone, regardless of whether they are an Oracle cloud user or not, to write objects to a bucket or delete objects. This option should not be configured unless there is a strong business requirement. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Object/Tasks/managingbuckets.htm |
| **Recommended Action** | Disable global all users policies on all object store buckets and ensure the bucket is configured with the least privileges. |

## Detailed Remediation Steps

