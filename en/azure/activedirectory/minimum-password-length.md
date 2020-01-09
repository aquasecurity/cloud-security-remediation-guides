[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Minimum Password Length

## Quick Info

| | |
|-|-|
| **Plugin Title** | Minimum Password Length |
| **Cloud** | AZURE |
| **Category** | Active Directory |
| **Description** | Ensures that all Azure passwords require a minimum length |
| **More Info** | Azure handles most password policy settings, including the minimum password length, defaulted to 8 characters. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts |
| **Recommended Action** | No action necessary. Azure handles password requirement settings. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Azure Active Directory. </br> <img src="/resources/azure/activedirectory/minimum-password-length/step2.png"/>
3.  Select the "Azure Active Directory."  On the navigation panel, select the "Users" under Manage option.</br> <img src="/resources/azure/activedirectory/minimum-password-length/step3.png"/>
4. On the "Users" tab click on the "New User" option at the top.</br> <img src="/resources/azure/activedirectory/minimum-password-length/step4.png"/>
5. On the "New User" tab, click on the "Create user."</br> <img src="/resources/azure/activedirectory/minimum-password-length/step5.png"/>
6. Under the "Identity", enter details like "Username","Name", "First Name","Last Name".</br> <img src="/resources/azure/activedirectory/minimum-password-length/step6.png"/>
7. On the "Password" tab, click on the "Let me create the password." </br> <img src="/resources/azure/activedirectory/minimum-password-length/step7.png"/>
8. On the "Initial Tab" enter the password, and if it's less than eight characters, Azure will show the error.</br> <img src="/resources/azure/activedirectory/minimum-password-length/step8.png"/>
9. Repeat the above steps to create New User with pre-defined "Minimum Password Length."</br>
