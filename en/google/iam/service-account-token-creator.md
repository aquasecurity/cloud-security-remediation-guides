[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / IAM / Service Account Token Creator

## Quick Info

| | |
|-|-|
| **Plugin Title** | Service Account Token Creator |
| **Cloud** | GOOGLE |
| **Category** | IAM |
| **Description** | Ensures that no users have the Service Account Token Creator role. |
| **More Info** | For best security practices, IAM users should not have Service Account Token Creator role. |
| **GOOGLE Link** | https://cloud.google.com/iam/docs/overview |
| **Recommended Action** | Ensure that no IAM user have Service Account Token Creator Role at GCP project level.|

## Detailed Remediation Steps
1. In the Google Cloud console, go to the IAM page.

    - [Go to IAM](https://console.cloud.google.com/projectselector/iam-admin/iam?supportedpurview=project,folder,organizationId)

2. Select a project by clicking on the project's name. 

3. Find the row containing the principal whose access you want to revoke. 

4. Click Edit principal in that row.

    - Note: You cannot edit inherited roles when managing access to a resource. To edit inherited roles, go to the resource where the role was granted.

5. Click the Delete delete button for the role that you want to revoke, and then click Save.
