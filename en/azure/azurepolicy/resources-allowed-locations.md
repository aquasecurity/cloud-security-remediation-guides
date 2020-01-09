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
3. On the "Policy" page, scroll down the left navigation panel and choose "Assignments" under "Authoring."</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step3.png"/>
4. On the "Policy - Assignments" page, check the "Policies" listed and if there are no "Policies" for "Resources Allowed Locations" then the selected "Assignment" don't have any "Resources Allowed Locations" policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step4.png"/>
5. Repeat steps number 2 - 4 to check different "Policy - Assignments."</br>
6. Navigate to "Policy", scroll down the left navigation panel and choose "Assignemts" and on the "Policy - Assignments" page click on the "Assign Policy" at the top to assign "Resource Allowed Location" policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step6.png"/>
7. On the "Assign Policy" page, select the "Scope" accordingly and click on the "..." dots icon to select the "Policy definition" under the "Basics" option.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step7.png"/>
8. On the "Available Definitions" page, click on the "Search" box at the tab and search for "Allowed locations for resource groups" and click on the "Select" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step8.png"/>
9. Provide the "Description" accordingly and click on the "Next" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step9.png"/>
10. On the "Parameters" tab, select the "Allowed location" from the dropdown menu accordingly and click on the "Next" button.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step10.png"/>
11. On the "Remediation" page, click on the checkbox next to the "Create a Managed Identity" and select the "Managed Identity Location" accordingly.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step11.png"/>
12. Click on the "Review + Create" button to create the specific "Resources Allowed Locations" policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step12.png"/>
13. Repeat steps number 6 - 12 to ensure that all services contain policy definitions that defined allowed locations.</br>
