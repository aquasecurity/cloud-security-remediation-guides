[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Scale Sets vTPM Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets vTPM Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that Virtual Trusted Platform Module (vTPM) is enabled for Virtual Machine Scale Sets. |
| **More Info** | vTPM is TPM2.0 compliant and enhances security by validating VM boot integrity and providing a secure storage mechanism for keys and secrets. The vTPM enables attestation by measuring the entire boot chain of your VM (UEFI, OS, system, and drivers). |
| **AZURE Link** | https://learn.microsoft.com/en-us/windows/security/hardware-security/tpm/trusted-platform-module-overview |
| **Recommended Action** | Modify virtual machine scale set configurations and enable vTPM |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. In the left-hand menu, go to "Disks", then select the OS disk used by the scale set.
5. Under the Security Type section, ensure "Trusted Launch Virtual Machines" is enabled. Toggle vTPM to "Enabled" and click Save. Restart the scale set to apply the changes.
6. Repeat steps 3-5 for all applicable scale set instances.