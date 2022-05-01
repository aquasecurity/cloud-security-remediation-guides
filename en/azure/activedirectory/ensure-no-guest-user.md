[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Ensure No Guest User

## Quick Info

| | |
|-|-|
| **Plugin Title** | Ensure No Guest User |
| **Cloud** | AZURE |
| **Category** | Active Directory |
| **Description** | Ensures that there are no guest users in the subscription |
| **More Info** | Guest users are usually users that are invited from outside the company structure, these users are not part of the onboarding/offboarding process and could be overlooked, causing security vulnerabilities. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/b2b/add-users-administrator |
| **Recommended Action** | Remove all guest users unless they are required to be members of the Active Directory account. |

## Detailed Remediation Steps


1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Azure Active Directory. </br> <img src="/resources/azure/activedirectory/ensure-no-guest-user/step2.png"/>
3.  Select the "Azure Active Directory" and on the left navigation panel, select the "Users" under "Manage".</br> <img src="/resources/azure/activedirectory/ensure-no-guest-user/step3.png"/>


