[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Logging / Audit Configuration Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | Audit Configuration Logging |
| **Cloud** | GOOGLE |
| **Category** | Logging |
| **Description** | Ensures that logging and log alerts exist for audit configuration changes. |
| **More Info** | Project Ownership is the highest level of privilege on a project, any changes in audit configuration should be heavily monitored to prevent unauthorized changes. |
| **GOOGLE Link** | https://cloud.google.com/logging/docs/logs-based-metrics/ |
| **Recommended Action** | Ensure that log alerts exist for audit configuration changes. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Logging" option under the "STACKDRIVER."</br> <img src="/resources/google/logging/audit-configuration-logging/step2.png"/>
3. On the "Stack driver Logging" page, click on the dropdown menu below the "CREATE METRIC" and choose the "Metric type" from the menu to choose the "Audit Configuration Changes."</br> <img src="/resources/google/logging/audit-configuration-logging/step3.png"/>
4. If the "Audit Configuration changes" contains no logs information, then the selected metric don't have logging and log alerts exist for audit configuration changes.</br> <img src="/resources/google/logging/audit-configuration-logging/step4.png"/>
5. Repeat steps number 2 - 4 to check other "Metric type" in the accounts.</br>
6. Navigate to the "Logging" option under the "STACKDRIVER", click on the dropdown menu below the "CREATE METRIC" and choose the "Metric type" from the menu to choose the "Audit Configuration Changes" to create a new metric for logging and log alerts.</br> <img src="/resources/google/logging/audit-configuration-logging/step6.png"/>
7. Click on the "CREATE METRIC" at the top to create a new metric.</br> <img src="/resources/google/logging/audit-configuration-logging/step7.png"/>
8. On the "Metric editor" tab, enter the "Name" and "Description" accordingly and enter the field name under the "Label" as per the requirements and click on the "Done" button to save the "Label."</br> <img src="/resources/google/logging/audit-configuration-logging/step8.png"/>
9. Click on the "Create metric" button at the bottom to make the changes.</br> <img src="/resources/google/logging/audit-configuration-logging/step9.png"/>
10. Repeat steps number 6 - 9 to ensure that log alerts exist for audit configuration changes.</br>
