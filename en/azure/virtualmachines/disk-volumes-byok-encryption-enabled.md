[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Disk Volumes BYOK Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk Volumes BYOK Encryption Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Azure virtual machine disks have BYOK (Customer-Managed Key) encryption enabled. |
| **More Info** | Encrypting virtual machine disk volumes helps protect and safeguard your data to meet organizational security and compliance commitments. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/windows/disk-encryption-key-vault |
| **Recommended Action** | Ensure that virtual machine disks are created using BYOK encryption. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines.
3. Select the corresponding virtual machine by clicking on the "Name" link.
4. In the left side menu, select "Disk" and click on the corresponding disk "Name" link.
5. In the left side menu, select "Encryption" and change the Encryption type to one of the customer-managed key options. Select the appropriate encryption sets and then click "Save" to confirm the changes.
6. Note that if no encryption sets are available, you will need to configure both the Azure "Key Vaults" as well as the "Disk Encryption Sets" resources. Please visit https://docs.microsoft.com/en-us/azure/virtual-machines/windows/disk-encryption-key-vault for more information. 
7. Repeat steps 3 - 6 for all other applicable virtual machines.