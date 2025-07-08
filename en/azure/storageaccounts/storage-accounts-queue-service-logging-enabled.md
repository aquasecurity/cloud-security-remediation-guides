
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Network Access Default Action

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Accounts Queue Service Logging Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Microsoft Azure Storage Queue service logging is enabled for "Read", "Write", and "Delete" requests. |
| **More Info** | Azure Storage Queue logs contain detailed information about successful and failed requests made to your storage queues for read, write and delete operations. This information can be used to monitor individual requests and to diagnose issues with the Storage Queue service within your Microsoft Azure account. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/queues/monitor-queue-storage?tabs=azure-portal |
| **Recommended Action** | Modify Queue Service and enable storage logging for "Read", "Write", and "Delete" requests. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts".</br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step3.png"/>
4. On the "Storage account" page, scroll down the left navigation panel and choose "Diagnostic Settings" under "Monitoring". </br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step4.png"/>
5. On the Diagnostic Settings page, select the "queue" service to configure its diagnostics. </br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step5.png"/>
6. Click Add diagnostic setting to create a new logging configuration. </br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step6.png"/>
7. In the Log categories section, either enable the individual options (Storage Read, Storage Write, and Storage Delete) or select allLogs to enable all categories at once. </br> <img src="/resources/azure/storageaccounts/storage-accounts-queue-service-logging-enabled/step7.png"/>