[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Microsoft Entra ID / Password Requires Numbers

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Numbers |
| **Cloud** | AZURE |
| **Category** | Microsoft Entra ID |
| **Description** | Ensures that all Azure passwords require numbers |
| **More Info** | Microsoft Entra ID handles most password policy settings, including which character types are required. It enforces at least three out of four of the following character types: lowercase, uppercase, special characters, and numbers. |
| **AZURE Link** | https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps
1. Log into Microsoft Entra Admin Center.
2. Select the "Search resources, services, and docs" option at the top and search for Microsoft Entra ID. 
3.  Select "Microsoft Entra ID". On the navigation panel, select "Users" under the Manage section.
4. On the "Users" tab click on the "New User" option at the top.
5. On the "New User" tab, click on the "Create user".
6. Under the "Identity", enter details like "Username","Name", "First Name","Last Name". Select the group if required and define the role for the user.
7. On the "Password" tab, click on the "Let me create the password".
8. If the password does not contain a number, Microsoft Entra ID will automatically display an error message when you click the "Create" button.
9. Repeat the above steps to create New User with pre-defined "Password Requires Numbers".
