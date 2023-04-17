[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Detailed Audit Logging Mode

## Quick Info

| | |
|-|-|
| **Plugin Title** | Detailed Audit Logging Mode |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Detailed Audit Logging Mode" policy is configured at the GCP organization level. |
| **More Info** | Detailed Audit Logging Mode is highly encouraged in coordination with Bucket Lock when seeking compliances such as SEC Rule 17a-4(f), CFTC Rule 1.31(c)-(d), and FINRA Rule 4511(c). |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that "Detailed Audit Logging Mode" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br></br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br></br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step2.png"/></br>
3. Navigate to [Identity and Access Management IAM](https://console.cloud.google.com/iam-admin/iam).
4. In the left navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step4.png"/></br></br>
5. Click inside Filter box, filter by **Name**. </br>
6. Type in **Detailed Audit Logging Mode** to return the \"Detailed Audit Logging Mode\" policy.</br><img src="/resources/google/resourcemanager/disable-service-account-key-creation/step6.png"/></br></br>
7. Click on the policy name. </br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step7.png"/></br></br>
8. On the Policy details page, check the **Status** attribute value. If the **Status** attribute value is set to **Not enforced**, then click on \"Manage Policy\" to edit the policy.</br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step8.png"/></br></br>
9. In Edit Policy screen, under \"Applies to\" section, select \"Customize\". Then Click on \"Add Role\".
10. In Add Role expanded Section, under enforcemnt: Select "On".</br></br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step10.png"/></br>
11. Click Save. </br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step11.png"/></br>
12. When return to Policy details screen, status will now show "Enforced". </br> <img src="/resources/google/resourcemanager/disable-service-account-key-creation/step12.png"/></br>