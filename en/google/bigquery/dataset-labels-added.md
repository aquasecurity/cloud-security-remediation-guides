[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / BigQuery / Dataset Labels Added

## Quick Info

| | |
|-|-|
| **Plugin Title** | Dataset Labels Added |
| **Cloud** | GOOGLE |
| **Category** | BigQuery |
| **Description** | Ensure that all BigQuery datasets have labels added. |
| **More Info** | Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage. |
| **GOOGLE Link** | https://cloud.google.com/bigquery/docs/adding-labels |
| **Recommended Action** | Ensure labels are added to all BigQuery datasets. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "BigQuery". </br> <img src="/resources/google/bigquery/dataset-labels-added/step2.png">
3. On the "SQL Workspace" page, click on the arrow on the left of your project id node to expand it.</br> <img src="/resources/google/bigquery/dataset-labels-added/step3.png"/>
4. Select the dataset which needs to be verified whether it has labels added or not by clicking on the dataset name.</br> <img src="/resources/google/bigquery/dataset-labels-added/step4.png"/>
5. On the right side, a panel will open with your dataset details. Under "Dataset Info", check if there is a "Labels" field. If the "Labels" field is not there or empty then the dataset does not have labels added.</br> <img src="/resources/google/bigquery/dataset-labels-added/step5.png"/>
6. Repeat steps number 4-5 to check other datasets in the project.</br>
7. Navigate to "BigQuery", click on the project node and click on the "Dataset" which needs to have labels added.</br> <img src="/resources/google/bigquery/dataset-labels-added/step7.png"/>
8. On the right side, a panel will open with your dataset details, click on "Edit Details".</br> <img src="/resources/google/bigquery/dataset-labels-added/step8.png"/>
9. Under "Labels", click on "Add Labels".</br> <img src="/resources/google/bigquery/dataset-labels-added/step9.png"/>
10. Add key and value for the label, add as many labels as you want and then click "Save".</br> <img src="/resources/google/bigquery/dataset-labels-added/step10.png"/>
11. Repeat steps number 7-10 to add labels to all other datasets in the project.</br>