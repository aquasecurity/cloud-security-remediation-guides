[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Disable Service Account Creation

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disable Service Account Creation |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Disable Service Account Creation" policy is enforced at the GCP organization level. |
| **More Info** | Enforcing the "Disable Service Account Creation" policy allows you to centrally manage your service accounts and reduces the chances of compromised service accounts being used to access your GCP resources. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** |Ensure that "Disable Service Account Creation" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br></br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br></br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step2.png"/></br>
3. Navigate to Cloud [Identity and Access Management IAM](https://console.cloud.google.com/iam-admin/iam).
4. In the left navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step4.png"/></br></br>
5. Click inside Filter box, filter by **Name**. </br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step5.png"/></br></br>
6. Type in **Disable Service Account Creation** to return the \"Disable Service Account Creation\" policy.</br>
7. Click on the policy name. </br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step7.png"/></br></br>
8. On the Policy details page, check the **Status** attribute value. If the **Status** attribute value is set to **Not enforced**, then click on \"Manage Policy\" to edit the policy.</br> <img src="/resources/google/resourcemanager/disable-service-account-creation/step8.png"/></br>