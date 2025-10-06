[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Entra ID / Password Requires Symbols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Symbols |
| **Cloud** | AZURE |
| **Category** | Entra ID |
| **Description** | Ensures that all Azure passwords require symbol characters |
| **More Info** | Azure handles most password policy settings, including which character types are required. Azure requires 3 out of 4 of the following character types: lowercase, uppercase, special characters, and numbers. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Entra ID. </br> <img src="/resources/azure/entraid/password-requires-symbols/step2.png"/>
3.  Select the "Azure Entra ID" and on the left navigation panel, select the "Users" under "Manage".</br> <img src="/resources/azure/entraid/password-requires-symbols/step3.png"/>
4. On the "Users" tab click on the "New User" option at the top.</br> <img src="/resources/azure/entraid/password-requires-symbols/step4.png"/>
5. On the "New User" page, select "Create user".</br> <img src="/resources/azure/entraid/password-requires-symbols/step5.png"/>
6. Under "Identity", enter details like "Username","Name", "First Name","Last Name".</br> <img src="/resources/azure/entraid/password-requires-symbols/step6.png"/>
7. Under "Password", click on "Let me create the password". </br> <img src="/resources/azure/entraid/password-requires-symbols/step7.png"/>
8. On the "Initial password" textbox enter the password, and if the password doesn't contain any "Symbols such as @, #", then the Azure will automatically show the error message "Unable to create user" when you will click "Create" button at the bottom.</br> <img src="/resources/azure/entraid/password-requires-symbols/step8.png"/>
9. If you click on the information bubble next to "Initial password" you will find the password combinations you can make.</br> <img src="/resources/azure/entraid/password-requires-symbols/step9.png"/>
10. Repeat the above steps to create New User with pre-defined "Password Requires Symbols".</br>
