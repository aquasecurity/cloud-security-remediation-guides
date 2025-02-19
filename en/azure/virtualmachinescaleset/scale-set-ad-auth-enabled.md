[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / Scale Sets AD Authentication Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Scale Sets AD Authentication Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that Azure Active Directory (AD) authentication is enabled for Virtual Machine Scale Sets. |
| **More Info** | Enabling Azure Active Directory (AD) authentication for VM Scale Sets ensures access from one central point and simplifies access permission management. It allows conditional access by using Role-Based Access Control (RBAC) policies, and enable MFA. |
| **AZURE Link** | https://learn.microsoft.com/en-us/entra/identity/devices/howto-vm-sign-in-azure-ad-linux |
| **Recommended Action** | Enable Active Directory authentication for all Virtual Machines scale sets. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. In the left-hand menu, navigate to "Identity" under the "Settings" section.
5. Under the System Assigned Identity tab, ensure that "Status" is set to On to enable Azure AD authentication.
6. Click "Save" to apply the changes.
7. Navigate to Azure Active Directory service in Azure portal.
8. Open "Enterprise Applications" > "Azure AD Domain Services", and ensure that the instances are added with the correct permissions.
9. Under VMSS portal, select "Configuration", and under "Login with Azure AD", ensure it is enabled.
10. Repeat steps 3-9 for all applicable scale set instances.