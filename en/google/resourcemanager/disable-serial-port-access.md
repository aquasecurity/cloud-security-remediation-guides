[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Disable Serial Port Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disable Serial Port Access |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if "Disable VM serial port access" policy is enforced at the GCP organization level. |
| **More Info** | For security purposes, ensure that serial port access to your VM instances is disabled. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** |Ensure that \"Disable VM serial port access\" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step2.png"/></br>
3. Navigate to Cloud [Identity and Access Management IAM] (https://console.cloud.google.com/iam-admin/iam).
4. In the left navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step4.png"/></br></br>
5. Click inside Filter box, filter by **Name**. </br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step5.png"/></br></br>
6. Type in **Disable VM serial port access** to return the \"Disable VM serial port access\" policy.</br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step6.png"/></br></br>
7. Click on the policy name. </br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step7.png"/></br></br>
8. On the Policy details page, check the **Status** attribute value. If the **Status** attribute value is set to **Not enforced**, then click on Manage Policy to edit the policy.</br> <img src="/resources/google/resourcemanager/disable-serial-port-access/step8.png"/></br>