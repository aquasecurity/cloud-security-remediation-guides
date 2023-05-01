[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Azure AD App Organisational Directory Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Azure AD App Organisational Directory Access |
| **Cloud** | AZURE |
| **Category** | Active Directory |
| **Description** | Ensures that Azure Active Directory applications are accessible to accounts in organisational directory only. |
| **More Info** | AAD provides different types of account access. By using single-tenant authentication, the impact gets limited to the application’s tenant i.e. all users from the same tenant could connect to the application and save app from unauthorised access. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/active-directory/develop/single-and-multi-tenant-apps |
| **Recommended Action** | Modify the Azure app authentication setting and provide access to accounts in organisational directory only. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Active Directory and Select the "Azure Active Directory" </br> <img src="/resources/azure/activedirectory/app-orgnaizational-directory-access/step2.png"/>
3. On the Active Directory Overview page Click on "App Registration" under "Manage" from left navigation panel.</br> <img src="/resources/azure/activedirectory/app-orgnaizational-directory-access/step3.png"/>
4. On App Registrations page Click on the App name for which you want to change the access.</br> <img src="/resources/azure/activedirectory/app-orgnaizational-directory-access/step4.png"/>
5. On App details page Click on "Authentication" under the "Manage" section from left navigation panel.</br> <img src="/resources/azure/activedirectory/app-orgnaizational-directory-access/step5.png"/>
6. On Authentication details page under the "Supported Account Types" select multi-tenant access and Click "Save" on the bottom of the page.</br> <img src="/resources/azure/activedirectory/app-orgnaizational-directory-access/step6.png"/>

