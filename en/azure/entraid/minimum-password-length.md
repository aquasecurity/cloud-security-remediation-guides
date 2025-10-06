[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Entra ID / Minimum Password Length

## Quick Info

| | |
|-|-|
| **Plugin Title** | Minimum Password Length |
| **Cloud** | AZURE |
| **Category** | Entra ID |
| **Description** | Ensures that all Azure passwords require a minimum length |
| **More Info** | Azure handles most password policy settings, including the minimum password length, defaulted to 8 characters. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Entra ID. </br> <img src="/resources/azure/entraid/minimum-password-length/step2.png"/>
3.  Select the "Azure Entra ID" and on the left navigation panel, select the "Users" under "Manage" .</br> <img src="/resources/azure/entraid/minimum-password-length/step3.png"/>
4. On the "Users" tab click on the "New User" tab at the top.</br> <img src="/resources/azure/entraid/minimum-password-length/step4.png"/>
5. On the "New User" page, select the option "Create user".</br> <img src="/resources/azure/entraid/minimum-password-length/step5.png"/>
6. Under the "Identity", enter details like "Username","Name", "First Name","Last Name".</br> <img src="/resources/azure/entraid/minimum-password-length/step6.png"/>
7. Under the "Password", select "Let me create the password". </br> <img src="/resources/azure/entraid/minimum-password-length/step7.png"/>
8. In the "Initial password" textbox enter the password, and if it's less than eight characters, Azure will show this error "The value must have a length of at least 8".</br> <img src="/resources/azure/entraid/minimum-password-length/step8.png"/>
9. Repeat the above steps to create New User with pre-defined "Minimum Password Length."</br>
