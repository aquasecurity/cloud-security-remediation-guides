[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Restrict Shared VPC Subnetworks

## Quick Info

| | |
|-|-|
| **Plugin Title** | Restrict Shared VPC Subnetworks |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if \"Restrict Shared VPC Subnetworks\" is enforced on the GCP organization level. |
| **More Info** | Enforcing the \"Restrict Shared VPC Subnetworks\" constraint allows you to define which VPC Shared Subnetworks your resources can use within your GCP organization. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that \"Restrict Shared VPC Subnetworks\" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to the Google Cloud console, go to the [Identity and Access Management (IAM)](#https://console.cloud.google.com/iam-admin/iam.) page.

2. Click on the deployment selector from the top navigation bar, select ALL to list all the existing deployments, then choose the Google Cloud organization that you want to examine.

3. In the navigation panel, select **Organization Policies** to view the list of the cloud organization policies available.

4. In the Filter by constraint section, select `Name` and filter by: `Restrict Shared VPC Subnetworks`.

5. Select the `Restrict Shared VPC Subnetworks` organizational policy. 

6. In the `Policy details` page, see the `Allowed` configuration attribute value. If the value is set to `All`, select the Manage Policy button in the upper right to modify the policy.

6. In the `Applies to` section, change the selection to Customize. 
 
7. Under `Policy enforcement` select Merge with parent.

8. Under the Rules section, select `Add rule` and provide a custom policy value to define allowed where cloud resources can be created. Once completed, select Done and Save. 