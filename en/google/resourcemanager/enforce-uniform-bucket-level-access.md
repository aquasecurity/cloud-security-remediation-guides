[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Enforce Uniform Bucket-Level Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enforce Uniform Bucket-Level Access |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Enforce uniform bucket-level access" policy is enabled at the GCP organization level. |
| **More Info** | Enforcing Uniform Bucket Level Access ensures that access is granted exclusively through Cloud IAM service which is more efficient and secure. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that "Enforce uniform bucket-level access" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br></br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br></br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step2.png"/></br>
3. Navigate to [Identity and Access Management IAM](https://console.cloud.google.com/iam-admin/iam).
4. In the left navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step4.png"/></br></br>
5. Click inside Filter box, filter by **Name**. </br>
6. Type in **Enforce uniform bucket-level access** to return the \"Enforce uniform bucket-level access\" policy.</br><img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step6.png"/></br></br>
7. Click on the policy name. </br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step7.png"/></br></br>
8. On the Policy details page, check the **Status** attribute value. If the **Status** attribute value is set to **Not enforced**, then click on \"Manage Policy\" to edit the policy.</br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step8.png"/></br></br>
9. In Edit Policy screen, under \"Applies to\" section, select \"Customize\". Then Click on \"Add Role\".
10. In Add Role expanded Section, under enforcemnt: Select "On".</br></br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step10.png"/></br>
11. Click Save. </br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step11.png"/></br>
12. When return to Policy details screen, status will now show "Enforced". </br> <img src="/resources/google/resourcemanager/enforce-uniform-bucket-level-access/step12.png"/></br>