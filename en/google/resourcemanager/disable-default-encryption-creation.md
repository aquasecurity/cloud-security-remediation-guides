[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Disable Default Encryption Creation

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disable Default Encryption Creation |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Restrict Default Google-Managed Encryption for Cloud SQL Instances" is enforced on the GCP organization level. |
| **More Info** | Google-managed encryption keys for Cloud SQL database instances to enforce the use of Customer-Managed Keys (CMKs) in order to have complete control over database encryption/decryption process. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that "Restrict Default Google-Managed Encryption for Cloud SQL Instances" constraint is enforced at the organization level. |

## Detailed Remediation Steps
**Note**</br>
\"Restrict default Google-managed encryption on Cloud SQL instances\" policy is being deprecated by Google Cloud, therefore the policy may not appear in your account. </br>
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br></br> <img src="/resources/google/resourcemanager/disable-default-encryption-creation/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br></br> <img src="/resources/google/resourcemanager/disable-default-encryption-creation/step2.png"/></br>
3. Navigate to [Identity and Access Management IAM](https://console.cloud.google.com/iam-admin/iam).
4. In the left navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/disable-default-encryption-creation/step4.png"/></br></br>
5. Click inside Filter box, filter by **Name**. </br>
6. Type in **Restrict Default Google-Managed Encryption for Cloud SQL Instances** to return the \"Restrict Default Google-Managed Encryption for Cloud SQL Instances\" policy.
7. Click on the policy name. 
8. On the Policy details page, check the **Status** attribute value. If the **Status** attribute value is set to **Not enforced**, then click on \"Manage Policy\" to edit the policy.
9. In Edit Policy screen, under \"Applies to\" section, select \"Customize\". Then Click on \"Add Role\".
10. In Add Role expanded Section, under enforcemnt: Select "On".</br></br> <img src="/resources/google/resourcemanager/disable-default-encryption-creation/step10.png"/></br>
11. Click Save. </br> <img src="/resources/google/resourcemanager/disable-default-encryption-creation/step11.png"/></br>
12. When return to Policy details screen, status will now show "Enforced".