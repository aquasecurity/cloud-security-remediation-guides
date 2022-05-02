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
2. Find the search bar at the top and search for Policy. </br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step2.png"/>
3. On the "Policy" page, scroll down the left navigation panel and choose "Assignments" under "Authoring".</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step3.png"/>
4. On the "Policy - Assignments" page, check the "Policies" listed and if there are no "Policies" for "Resources Allowed Locations" then the selected "Assignment" don't have any "Resources Allowed Locations" policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step4.png"/>
5. If there is no policy for "Resources Allowed Locations" then click on "Assign policy" at the top to create a new policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step5.png"/>
6. On the "Assign Policy" page, under "Basics" tab, select "Scope" accordingly and click on the "..." dots icon next to "Policy definition".</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step6.png"/>
7. On the "Available Definitions" page, click on the "Search" box and search for "Resources Allowed Locations". Click the Policy Definition found and then click "Select" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step7.png"/>
8. Once back on the "Assign Policy" page, provide a "Description" and click on the "Next" button at the bottom. Now select "Allowed locations" on "Parameters" tab and click Next at the bottom.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step8.png"/>
9. On the "Remediation" tab, click on the checkbox next to the "Create a Managed Identity" and select desired "Managed Identity Location". Click "Review + create" button at the bottom.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step9.png"/>
10. On the "Review + Create" tab, click "Create" button at the bottom to create the specific "Resources Allowed Locations" policy.</br> <img src="/resources/azure/azurepolicy/resources-allowed-locations/step10.png"/>
11. Repeat steps number 6 - 10 to enable the built-in Azure Policy definition: Audit Resources Allowed Locations for all directories.</br>
