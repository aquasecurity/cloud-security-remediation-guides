[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Password Authentication Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Authentication Disabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that password authentication is disabled on Azure virtual machines. |
| **More Info** | SSH provides secure sign-ins over unsecured connections. Although SSH provides an encrypted connection, using passwords with SSH connections still leaves the VM vulnerable so it is recommended to connect to VM over SSH instead of password. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/linux/create-ssh-keys-detailed |
| **Recommended Action** | Disable password authentication on Azure virtual machine. |

## Detailed Remediation Steps

1. Option 1: Change the virtual machine's SSH configuration file to indicate "disable_password_authentication = true"
2. Option 2: SSH Authentication can be set at build time instead of password authentication. Rebuilding or migrating machines where feasible would satisfy this requirement. 
