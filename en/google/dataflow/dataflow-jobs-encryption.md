[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Dataflow / Dataflow Jobs Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Dataflow Jobs Encryption |
| **Cloud** | GOOGLE |
| **Category** | Datflow |
| **Description** | Ensure that Google Dataflow jobs are encrypted with desired encryption level. |
| **More Info** | Google encrypts all jobs in Dataflow by default. Protecting source and sinks data for Dataflow batch pipeline with CMEK gives user more granular access to encryption and decryption process.|
| **GOOGLE Link** | https://cloud.google.com/dataflow/docs/guides/customer-managed-encryption-keys |
| **Recommended Action** | Use desired encryption level to encrypt Dataflow jobs. |

## Detailed Remediation Steps
1.  Open the Dataflow monitoring UI.\
    [Go to the Dataflow Web UI](https://console.cloud.google.com/dataflow)
2.  Select Create job from template.
3.  In the Encryption section, select Customer-managed key.

Note: The drop-down menu Select a customer-managed key only shows keys with the regional scope global or the region you selected in the Regional endpoint drop-down menu. In order to minimize Cloud KMS operation latency and improve system availability, we recommend choosing regional keys.

The first time you attempt to run a job with a particular Cloud KMS key, your Compute Engine service account and/or Dataflow service account might not have been granted the permissions to encrypt and decrypt using that key. In this case, a warning message appears to prompt you to grant the permission to your service account.
