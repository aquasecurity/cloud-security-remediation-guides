[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Azure Policy / Resources Allowed Locations

## Quick Info

| | |
|-|-|
| **Plugin Title** | Resources Allowed Locations |
| **Cloud** | AZURE |
| **Category** | Azure Policy |
| **Description** | Ensures deployed resources and resource groups belong to the list set in the allowed locations for resource groups policy |
| **More Info** | Setting allowed locations for a service helps ensure the service can only be deployed in expected locations. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/governance/policy/assign-policy-portal |
| **Recommended Action** | Ensure that all services contain policy definitions that defined allowed locations. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Policy. </br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step2.png"/>
3. On the "Policy" page, scroll down the left navigation panel and choose "Assignments" under "Authoring."</br>
4. On the "Policy - Assignments" page, check the "Policies" listed and if there are no "Policies" for "Resources Allowed Locations" then the selected "Assignment" don't have any "Resources Allowed Locations" policy.</br>
5. Repeat steps number 2 - 4 to check different "Policy - Assignments."</br>
6. 
