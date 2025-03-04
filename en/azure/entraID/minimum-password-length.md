[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Microsoft Entra ID / Minimum Password Length

## Quick Info

| | |
|-|-|
| **Plugin Title** | Minimum Password Length |
| **Cloud** | AZURE |
| **Category** | Microsoft Entra ID |
| **Description** | Ensures that all Azure passwords require a minimum length |
| **More Info** | Microsoft Entra ID handles most password policy settings, including the minimum password length, defaulted to 8 characters. |
| **AZURE Link** | https://learn.microsoft.com/en-us/entra/identity/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Microsoft Entra ID handles password requirement settings. |

## Detailed Remediation Steps
1. Log in to the Microsoft Entra admin center.
2. Find the search bar at the top and search for Microsoft Entra ID.
3.  Select "Microsoft Entra ID" and on the left navigation panel, select "Users" under "Manage".
4. On the "Users" tab click on the "New User" tab at the top.
5. On the "New User" page, select the option "Create user".
6. Under the "Identity", enter details like "Username","Name", "First Name","Last Name".
7. Under the "Password", select "Let me create the password".
8. In the "Initial password" textbox, enter the password. If it's less than eight characters, Microsoft Entra ID will show this error: "The value must have a length of at least 8".
9. Repeat the above steps to create New User with pre-defined "Minimum Password Length. 
