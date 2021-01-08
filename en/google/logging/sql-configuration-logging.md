[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Logging / SQL Configuration Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Configuration Logging |
| **Cloud** | GOOGLE |
| **Category** | Logging |
| **Description** | Ensures that logging and log alerts exist for SQL configuration changes |
| **More Info** | Project Ownership is the highest level of privilege on a project, any changes in SQL configurations should be heavily monitored to prevent unauthorized changes. |
| **GOOGLE Link** | https://cloud.google.com/logging/docs/logs-based-metrics/ |
| **Recommended Action** | Ensure that log alerts exist for SQL configuration changes. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Logging" option under the "STACKDRIVER."</br> <img src="/resources/google/logging/sql-configuration-logging/step2.png"/>
3. On the "Stack driver Logging" page, click on the "Logs-based metrics" option./br> <img src="/resources/google/logging/sql-configuration-logging/step3.png"/>
4. On the "Logs-based metric" page, search the "System metrics" and "User-defined metrics" and check whether any metrics is there for "SQL Configuration Logging." If no such metrics is present then the logging and log alerts does not exist for SQL configuration changes.</br> <img src="/resources/google/logging/sql-configuration-logging/step4.png"/>
5. Repeat steps number 2 - 4 to check other GCP accounts.</br>
6. Navigate to the "Logging" option under the "STACKDRIVER", choose the "Logbased metrics" and click on the "CREATE METRIC" button at the top.</br> <img src="/resources/google/logging/sql-configuration-logging/step6.png"/>
7. On the "Metric editor" tab, enter the "Name" and "Description" accordingly and enter the field name under the "Label" as per the requirements and click on the "Done" button to save the "Label."</br> <img src="/resources/google/logging/sql-configuration-logging/step7.png"/>
8. Click on the "Create metric" button at the bottom to make the changes.</br> <img src="/resources/google/logging/sql-configuration-logging/step8.png"/>
9. On the "Logs-based metrics", under the "User-defined metrics" click on the 3 dots next to the newly created "SQL Configuration Logging" metric and click on the "create alert from metric."</br> <img src="/resources/google/logging/sql-configuration-logging/step9.png"/>
10. On the "Create alert" page, select the "Aggregator" as per the requirement and select the "Configuration" from the dropdown menu accordingly.</br> <img src="/resources/google/logging/sql-configuration-logging/step10.png"/>
11. Enter the "Condition, Threshold and Minute" of the above "Configuration" accordingly and click on the "Save" button to make the changes.</br> <img src="/resources/google/logging/sql-configuration-logging/step11.png"/>
12. Once the settings are "Saved", enter the name of the alarm and select "Policy triggers" condition from the dropdown menu.</br> <img src="/resources/google/logging/sql-configuration-logging/step12.png"/>
13. Click on the "Save" button at the bottom to make the chanes.</br> <img src="/resources/google/logging/sql-configuration-logging/step13.png"/>
14. Repeat steps number 6 - 14 to ensure that log alerts exist for SQL configuration changes.</br>

