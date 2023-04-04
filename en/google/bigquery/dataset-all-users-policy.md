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