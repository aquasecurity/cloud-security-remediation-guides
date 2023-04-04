[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / BigQuery / Tables CMK Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Tables CMK Encrypted |
| **Cloud** | GOOGLE |
| **Category** | BigQuery |
| **Description** | Ensure that BigQuery dataset tables are encrypted using desired encryption protection level. |
| **More Info** | By default Google encrypts all dataset tables using Google-managed encryption keys. To have more control over the encryption process of your BigQuery dataset tables you can use Customer-Managed Keys (CMKs). |
| **GOOGLE Link** | https://cloud.google.com/bigquery/docs/dataset-access-controls |
| **Recommended Action** | Ensure that each BigQuery dataset table has desired encryption level. |

## Detailed Remediation Steps
1. To change a table from default encryption to Cloud KMS protection https://cloud.google.com/bigquery/docs/customer-managed-encryption#change_to_kms

To determine if a table is protected by Cloud KMS:
1. Sign in to Google Cloud Management Console.
2. Select the Google Cloud Platform (GCP) project that you want to examine from the console top navigation bar.
3. Navigate to Google Cloud BigQuery dashboard at https://console.cloud.google.com/bigquery.
4. In the Explorer pane, expand your project and select a dataset name, and click on the specific BigQuery table that you want to examine.
5. Select the Details tab to access the configuration details available for the selected table.
6. On the Details panel, within the Table info section, search for the Customer-managed key configuration attribute. If the Customer-managed key attribute is not listed in the table information section, the selected Google Cloud BigQuery dataset table is not encrypted using a Customer-Managed Key (CMK).