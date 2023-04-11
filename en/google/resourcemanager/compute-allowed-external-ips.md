[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Compute Allowed External IPs

## Quick Info

| | |
|-|-|
| **Plugin Title** | Compute Allowed External IPs |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if \"Define Allowed External IPs for VM Instances\" constraint policy is enabled at the GCP organization level. |
| **More Info** | To reduce exposure to the internet, make sure that not all VM instances are allowed to use external IP addresses. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that \"Define Allowed External IPs for VM Instances\" constraint is enforced to allow you to define the VM instances that are allowed to use external IP addresses. |

## Detailed Remediation Steps
1. Sign in to Google Cloud Management Console with the organizational unit credentials, then Click the deployment selector in the upper navigation bar.</br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step1.png"/></br>
2. Select ALL to view a summary of all current deployments, and then pick the Google Cloud organisation you want to look at.</br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step2.png"/></br>
3. Navigate to Cloud Identity and Access Management (IAM) [dashboard](#https://console.cloud.google.com/iam-admin/iam).
4. In the navigation panel, select Organization Policies to view the list of the constraint policies available for your GCP organization.</br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step4.png"/></br>
5. Click inside Filter box, select *Name* and *Define allowed external IPs for VM instances* to return the \"Define Allowed External IPs for VM Instances\" policy.</br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step5.png"/></br>
6. Click on the GCP organization policy returned at step 5.
7. On the Policy details page, check the **Allowed** configuration attribute value. If the **Allowed** attribute value is set to **All**, then all the virtual machine instances created within the selected Google Cloud Platform (GCP) organization are allowed to use external IP addresses.
8. Click on Manage Policy to define constraint policy.</br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step8.png"/></br>
9. In Edit Policy screen, under \"Applies to\" section, select \"Customize\". Then under policy enforcement: Select Replace. Finally, Click on \"Add Role\".</br></br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step9.png"/></br>
10. In Add Role expanded Section, for Policy Value: Select "\Deny All\". Then Click on "\Add Condition\"</br></br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step10.png"/></br>
11. In Edit Condition Screen, Add the required conditions to allow only VM instances taht needs to use external IP addresses </br> <img src="/resources/google/resourcemanager/compute-allowed-external-ips/step11.png"/></br>
12. Click Save.