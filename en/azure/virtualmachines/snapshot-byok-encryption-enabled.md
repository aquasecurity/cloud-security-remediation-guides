[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Disk Snapshot BYOK Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Disk Snapshot BYOK Encryption Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Azure virtual machine disk snapshot have BYOK (Customer-Managed Key) encryption enabled. |
| **More Info** | EEncrypting virtual machine disk snapshot helps protect and safeguard your data to meet organizational security and compliance commitments. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/virtual-machines/disk-encryption |
| **Recommended Action** | Modify affected snapshots and and enable Customer Managed key encryption |

## Detailed Remediation Steps


1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Snapshots. </br> <img src="/resources/azure/virtualmachines/snapshot-byok-encryption-enabled/step2.png"/>
3. Select the "Snapshot" by clicking the "Name" as a link to get into the configuration changes. </br> <img src="/resources/azure/virtualmachines/snapshot-byok-encryption-enabled/step3.png"/>
4. On "Snapshot" navigation panel and choose "Encryption" under the settings section. </br> <img src="/resources/azure/virtualmachines/snapshot-byok-encryption-enabled/step4.png"/>
5. Click on "Key Management" dropdown then select "Customer-managed key" and Click save from top navigation panel.</br> <img src="/resources/azure/virtualmachines/snapshot-byok-encryption-enabled/step5.png"/>