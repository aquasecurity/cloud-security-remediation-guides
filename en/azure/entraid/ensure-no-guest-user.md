[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Entra ID / Ensure No Guest User

## Quick Info

| | |
|-|-|
| **Plugin Title** | Ensure No Guest User |
| **Cloud** | AZURE |
| **Category** | Entra ID |
| **Description** | Ensures that there are no guest users in the subscription |
| **More Info** | Guest users are usually users that are invited from outside the company structure, these users are not part of the onboarding/offboarding process and could be overlooked, causing security vulnerabilities. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/b2b/add-users-administrator |
| **Recommended Action** | Remove all guest users unless they are required to be members of the Entra ID account. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Entra ID. </br> <img src="/resources/azure/entraid/ensure-no-guest-user/step2.png"/>
3. Select the "Azure Entra ID" and on the left navigation panel, select the "Users" under "Manage".</br> <img src="/resources/azure/entraid/ensure-no-guest-user/step3.png"/>
4. In the users list, look for users with "User type" as "Guest". If there are "Guest" type users then those users are not part of the onboarding/offboarding process and are considered a security vulnerability. Such accounts must be deleted.</br> <img src="/resources/azure/entraid/ensure-no-guest-user/step4.png"/>
5. Select all Users with "User type" as "Guest" and click "Delete User" on the top right.</br> <img src="/resources/azure/entraid/ensure-no-guest-user/step5.png"/>
6. Click OK in the confirmation popup.</br> <img src="/resources/azure/entraid/ensure-no-guest-user/step6.png"/>
7. Repeat step number 3 to 6 for all other directories.
