[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SQL CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL CMK Encryption |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensure that Cloud SQL instances are encrypted using Customer Managed Keys (CMKs). |
| **More Info** | By default, your Google Cloud SQL instances are encrypted using Google-managed keys. To have a better control over the encryption process of your Cloud SQL instances you can use Customer-Managed Keys (CMKs). |
| **GOOGLE Link** | "https://cloud.google.com/sql/docs/sqlserver/cmek" |
| **Recommended Action** | Ensure that all Google Cloud SQL instances have desired encryption level.|

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the Cloud SQL Instances page.

    [Go to Cloud SQL Instances](https://console.cloud.google.com/sql)

2.  In the Instances list, scroll to the right until you see the Encryption column. In this column, you see Google-managed and Customer-managed.
3.  Click an instance name to open its Overview page. The customer-managed encryption key is listed in the Configuration pane.
    - Note that Customer Managed Encryption Keys can only be configured during instance creation.
