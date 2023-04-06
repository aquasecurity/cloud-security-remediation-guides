[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Disable Automatic IAM Grants

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disable Automatic IAM Grants |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Disable Automatic IAM Grants for Default Service Accounts" policy is enforced at the organization level. |
| **More Info** | By default, service accounts get the editor role when created. To improve access security, disable the automatic IAM role grant. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that \"Disable Automatic IAM Grants for Default Service Accounts\" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials.
2. Click the deployment selector in the upper navigation bar, select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.
3. Navigate to Cloud Identity and Access Management (IAM) [dashboard](#https://console.cloud.google.com/iam-admin/iam).
4. In the navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/disable-automatic-iam-grants/step4.png"/></br>
5. Click inside Filter box, select **Name**. </br> <img src="/resources/google/resourcemanager/disable-automatic-iam-grants/step5.png"/></br>
6. Type in **Disable Automatic IAM Grants** to return the \"Disable Automatic IAM Grants\" policy.</br> <img src="/resources/google/resourcemanager/disable-automatic-iam-grants/step6.png"/></br>
7. Click on the GCP organization policy returned at step 6. </br> <img src="/resources/google/resourcemanager/disable-automatic-iam-grants/step7.png"/></br>
8. On the Policy details page, check the **Status** configuration attribute value. If the **Status** attribute value is set to **Not enforced**, then click on Manage Policy to edit the policy.</br> <img src="/resources/google/resourcemanager/disable-automatic-iam-grants/step8.png"/></br>