[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Guest Level Diagnostics Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Guest Level Diagnostics Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that the guest level diagnostics are enabled. |
| **More Info** | Guest Level Diagnostics should be enabled to collect information about VMs processing and state of VM applications. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-enable-vm-agent |
| **Recommended Action** | Enable guest level diagnostics for all virtual machines. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines.
3. Select the corresponding virtual machine by clicking on the "Name" link.
4. Ensure that the Virtual Machine is currently running.
5. In the left menu pane, select "Diagnostic settings" under Monitoring.
6. In the Diagnostic Settings Overview, select a storage account under "Pick a storage account" and then select "Enable guest-level monitoring".
7. Repeat steps 3 - 6 for all other applicable Virtual Machines.
