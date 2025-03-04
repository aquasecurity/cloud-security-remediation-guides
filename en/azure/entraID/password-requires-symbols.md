[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Microsoft Entra ID / Password Requires Symbols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Symbols |
| **Cloud** | AZURE |
| **Category** | Microsoft Entra ID |
| **Description** | Ensures that all Azure passwords require symbol characters |
| **More Info** | Azure handles most password policy settings, including which character types are required. Azure requires 3 out of 4 of the following character types: lowercase, uppercase, special characters, and numbers. |
| **AZURE Link** | hhttps://learn.microsoft.com/en-us/entra/identity/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps

1. Log into Microsoft Entra Admin Center.
2. Select the "Search resources, services, and docs" option at the top and search for Microsoft Entra ID. 
3.  Select "Microsoft Entra ID". On the navigation panel, select "Users" under the Manage section. 
4. On the "Users" tab click on the "New User" option at the top.
5. On the "New User" page, select "Create user".
6. Under "Identity", enter details like "Username","Name", "First Name","Last Name".
7. Under "Password", click on "Let me create the password".
8. On the "Initial password" textbox enter the password. If the password does not contain a number, Microsoft Entra ID will automatically display an error message when you click the "Create" button. 
9. If you click on the information bubble next to "Initial password" you will find the password combinations you can make.
10. Repeat the above steps to create New User with pre-defined "Password Requires Symbols".
