[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Storage Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Account Blob Service Logging Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Microsoft Azure Storage Blob service logging is enabled for "Read", "Write", and "Delete" requests. |
| **More Info** | Azure Storage Blob logs contain detailed information about successful and failed requests made to your storage blobs for read, write and delete operations. This information can be used to monitor individual requests and to diagnose issues with the Storage Blob service within your Microsoft Azure account. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/monitor-blob-storage?tabs=azure-portal |
| **Recommended Action** | Modify Blob Service and enable storage logging for "Read", "Write", and "Delete" requests.|

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts".</br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step3.png"/>
4. On the "Storage account" page, scroll down the left navigation panel and choose "Diagnostic Settings" under "Monitoring". </br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step4.png"/>
5. On the Diagnostic Settings page, select the "blob" service to configure its diagnostics. </br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step5.png"/>
6. Click Add diagnostic setting to create a new logging configuration. </br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step6.png"/>
7. In the Log categories section, either enable the individual options (Storage Read, Storage Write, and Storage Delete) or select allLogs to enable all categories at once. </br> <img src="/resources/azure/storageaccounts/blob-service-logging-enabled/step7.png"/>