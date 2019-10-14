[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Instance Max Count

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Max Count |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures the total number of VM instances does not exceed a set threshold. |
| **More Info** | The number of running VM instances should be carefully audited, especially in unused regions, to ensure only approved applications are consuming compute resources. Many compromised Oracle accounts see large numbers of VM instances launched. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Compute/Concepts/instancemanagement.htm |
| **Recommended Action** | Ensure that the number of running VM instances matches the expected count. If instances are launched above the threshold, investigate to ensure they are legitimate. |

## Detailed Remediation Steps

