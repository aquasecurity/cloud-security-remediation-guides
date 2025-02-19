[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Scale Sets Secure Boot Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets Secure Boot Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that secure boot is enabled for Virtual Machine Scale Sets. |
| **More Info** | Secure Boot, which is implemented in platform firmware, protects against the installation of malware-based rootkits and boot kits. Secure Boot works to ensure that only signed operating systems and drivers can boot. It establishes a "root of trust" for the software stack on your VMSS. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/virtual-machines/trusted-launch#secure-boot |
| **Recommended Action** | Modify virtual machine scale set configurations and enable secure boot. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. In the left-hand menu, go to "Disks", then select the OS disk used by the scale set.
5. Under the Security Type section, ensure "Trusted Launch Virtual Machines" is enabled. Toggle Secure Boot to "Enabled" and click Save. Restart the scale set to apply the changes.
6. Repeat steps 3-5 for all applicable scale set instances.