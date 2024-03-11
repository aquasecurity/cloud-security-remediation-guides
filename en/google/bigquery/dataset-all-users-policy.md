[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / BigQuery / Dataset All Users Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Dataset All Users Policy |
| **Cloud** | GOOGLE |
| **Category** | BigQuery |
| **Description** | Ensure that BigQuery datasets do not allow public read, write or delete access. |
| **More Info** | Granting permissions to allUsers or allAuthenticatedUsers allows anyone to access the dataset. Such access might not be desirable if sensitive data is being stored in the dataset. |
| **GOOGLE Link** | https://cloud.google.com/bigquery/docs/dataset-access-controls |
| **Recommended Action** | Ensure that each dataset is configured so that no member is set to allUsers or allAuthenticatedUsers. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "BigQuery".
3. In the Explorer pane, expand your project and select a dataset that allows public access.
4. Click Sharing then Permissions.
5. Review each attached role to find allUsers and/or allAuthenticatedUsers Roles.
6. Click on the role associated with the allUsers and/or allAuthenticatedUsers member to expand the role configuration panel.
7. Click the delete icon for each member of allUsers or allAuthenticatedUsers. On the popup click Remove to confirm your action.
8. Click Close to return to the selected BigQuery dataset dashboard.
9. Repeat step no. 4 – 7 for each publicly accessible dataset created within the selected project.
10. Repeat steps no. 3 – 9 for each project deployed in your Google Cloud account.
