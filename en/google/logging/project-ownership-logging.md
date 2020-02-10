[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Logging / Project Ownership Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | Project Ownership Logging |
| **Cloud** | GOOGLE |
| **Category** | Logging |
| **Description** | Ensures that logging and log alerts exist for project ownership assignments and changes |
| **More Info** | Project Ownership is the highest level of privilege on a project, any changes in project ownership should be heavily monitored to prevent unauthorized changes. |
| **GOOGLE Link** | https://cloud.google.com/logging/docs/logs-based-metrics/ |
| **Recommended Action** | Ensure that log alerts exist for project ownership assignments and changes. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Logging" option under the "STACKDRIVER."</br> <img src="/resources/google/logging/project-ownership-logging/step2.png"/>
3. On the "Stack driver Logging" page, click on the "Logs-based metrics" option./br> <img src="/resources/google/logging/project-ownership-logging/step3.png"/>
4. On the "Logs-based metric" page, search the "System metrics" and "User-defined metrics" and check whether any metrics is there for "Project Ownership Logging." If no such metrics is present then the logging and log alerts does not exist for project ownership assignments and changes.</br>
5. Repeat steps number 2 - 4 to check other GCP accounts.</br>
6. Navigate to the "Logging" option under the "STACKDRIVER", choose the "Logbased metrics" and click on the "CREATE METRIC" button at the top.</br>
7. On the "Metric editor" tab, enter the "Name" and "Description" accordingly and enter the field name under the "Label" as per the requirements and click on the "Done" button to save the "Label."</br> 
8. Click on the "Create metric" button at the bottom to make the changes.</br> 
9. On the "Logs-based metrics", under the "User-defined metrics" click on the 3 dots next to the newly created "Project Ownership Logging" metric and click on the "create alert from metric."</br>
