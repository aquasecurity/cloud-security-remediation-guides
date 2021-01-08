[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Logging / Log Sinks Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Sinks Enabled |
| **Cloud** | GOOGLE |
| **Category** | Logging |
| **Description** | Ensures a log sink is enabled to export all logs |
| **More Info** | Log sinks send log data to a storage service for archival and compliance. A log sink with no filter is necessary to ensure that all logs are being properly sent. If logs are sent to a storage bucket, the bucket must exist and bucket versioning should exist. |
| **GOOGLE Link** | https://cloud.google.com/logging/docs/export/ |
| **Recommended Action** | Ensure a log sink is configured properly with an empty filter and a destination. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Logging" option under the "STACKDRIVER."</br> <img src="/resources/google/logging/log-sinks-enabled/step2.png"/>
3. On the "Stackdriver Logging" page, choose the "Logs Router" option from the left navigation panel.</br> <img src="/resources/google/logging/log-sinks-enabled/step3.png"/>
4. Select the "Log Sink" which needs to be cross-check whether it's properly configured or not.</br> <img src="/resources/google/logging/log-sinks-enabled/step4.png"/>
5. On the selected "Log Sink", click on the 3 dots at the extreme right and choose the "View Filter" option.</br> <img src="/resources/google/logging/log-sinks-enabled/step5.png"/>
6. If the "Sink filter" tab is showing any filter option then the selected "Log Sink" is not configred with empty filter.</br> <img src="/resources/google/logging/log-sinks-enabled/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Log Sinks" in the account.</br>
8. Navigate to the "Logging" option under the "STACKDRIVER", click on the "Log Router" option and select the "Log Sink" which needs to be re-configured and click on the 3 dots at the extreme right to choose the "View filter" option.</br> <img src="/resources/google/logging/log-sinks-enabled/step8.png"/>
9. On the "View filter" tab, click on the "Edit" button to edit the "Log Sink."</br> <img src="/resources/google/logging/log-sinks-enabled/step9.png"/>
10. On the "Edit Sink" tab, remove the filter and click on the "Update Sink" button to make the changes.</br> <img src="/resources/google/logging/log-sinks-enabled/step10.png"/>
11. Click on the "OK" button on the popup tab to save the changes which will over write the previous filters enabled.</br> <img src="/resources/google/logging/log-sinks-enabled/step11.png"/>
12. Repeat steps number 8 - 11 to ensure a log sink is configured properly with an empty filter and a destination.</br> 

