[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Instances with No Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instances with No Access |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that instances are not configured to use the default service account with full access to all Cloud APIs. |
| **More Info** | To support principle of least privileges and prevent potential privilege escalation it is recommended that instances are not assigned to default service account Compute Engine default service account with Scope Allow full access to all Cloud APIs. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances |
| **Recommended Action** | In Service Account Section, ensure Allow full access to all Cloud APIs is not selected if selecting the default service account. |

## Detailed Remediation Steps

