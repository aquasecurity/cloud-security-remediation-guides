[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Azure Policy / Resource Location Matches Resource Group

## Quick Info

| | |
|-|-|
| **Plugin Title** | Resource Location Matches Resource Group |
| **Cloud** | AZURE |
| **Category** | Azure Policy |
| **Description** | Ensures a policy is configured to audit that deployed resource locations match their resource group locations |
| **More Info** | Using Azure Policy to monitor resource location compliance helps ensure that new resources are not launched into locations that do not match their resource group. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/governance/policy/assign-policy-portal |
| **Recommended Action** | Enable the built-in Azure Policy definition: Audit resource location matches resource group location |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Policy. </br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step2.png"/>
3. On the "Policy" page, scroll down the left navigation panel and choose "Assignments" under "Authoring".</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step3.png"/>
4. On the "Policy - Assignments" page, check the "Policies" listed and if there are no "Policies" for "Resource Location Matches Resource Group" then the selected "Assignment" don't have any "Resource Location Matches Resource Group" policy.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step4.png"/>
5. If there is no policy for "Resource Location Matches Resource Group" then click on "Asign policy" at the top to create a new policy.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step5.png"/>
6. On the "Assign Policy" page, select the "Scope" accordingly and click on the "..." dots icon to select the "Policy definition" under the "Basics" tab.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step6.png"/>
7. On the "Available Definitions" page, click on the "Search" box at the tab and search for "Resource Location Matches Resource Group" and click on the "Select" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step8.png"/>
8. Provide the "Description" accordingly and click on the "Next" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step9.png"/>
9. On the "Remediation" page, click on the checkbox next to the "Create a Managed Identity" and select the "Managed Identity Location" accordingly.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step11.png"/>
10. Click on the "Review + Create" button to create the specific "Resource Location Matches Resource Group" policy.</br> <img src="/resources/azure/azurepolicy/resource-location-matches-resource-group/step12.png"/>
11. Repeat steps number 6 - 10 to enable the built-in Azure Policy definition: Audit resource location matches resource group location for all directories.</br>
