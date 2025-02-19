[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / VM Scale Set Managed Identity Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Scale Set Managed Identity Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that Azure Virtual Machine Scale Sets have managed identity enabled. |
| **More Info** | Enabling managed identities eliminate the need for developers having to manage credentials by providing an identity for the Azure resource in Azure AD and using it to obtain Azure Active Directory (Azure AD) tokens. |
| **AZURE Link** | https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/qs-configure-portal-windows-vmss |
| **Recommended Action** | Modify VM Scale Set and enable managed identity.|

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link.
4. Under the System Assigned Identity tab, toggle "Status" to On and click Save.
5. If a User Assigned Identity is required, navigate to the User Assigned tab, click "Add", select the appropriate identity, and click Add.
6. Assign the necessary Azure Role-Based Access Control (RBAC) permissions to the managed identity by going to Azure Role Assignments and selecting the required roles.
7. Repeat steps 3-6 for all applicable scale set instances.