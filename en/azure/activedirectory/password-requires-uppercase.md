[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Password Requires Uppercase

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Uppercase |
| **Cloud** | AZURE |
| **Category** | Active Directory |
| **Description** | Ensures that all Azure passwords require uppercase characters |
| **More Info** | Azure handles most password policy settings, including which character types are required. Azure requires 3 out of 4 of the following character types: lowercase, uppercase, special characters, and numbers. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Active Directory. </br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step2.png"/>
3. Select the "Azure Active Directory" and on the left navigation panel, select the "Users" under "Manage".</br><img src="/resources/azure/activedirectory/password-requires-uppercase/step3.png"/>
4. On the "Users" tab click on "New User" option at the top.</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step4.png"/>
5. On the "New User" page, select "Create user."</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step5.png"/>
6. Under "Identity", enter details like "Username","Name", "First Name","Last Name".</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step6.png"/>
7. Under "Password", select "Let me create the password".</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step7.png"/>
8. In the "Initial password" textbox enter the password, and if the password doesn't contain any uppercase characters then the Azure will automatically show the error message "Unable to create user" when you click on "Create" button at the botton.</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step8.png"/>
9. If you click on the information bubble next to "Initial password" you will find the password combinations you can make.</br> <img src="/resources/azure/activedirectory/password-requires-uppercase/step9.png"/>
10. Repeat the above steps to create New User with pre-defined "Password Requires Uppercase."</br>
