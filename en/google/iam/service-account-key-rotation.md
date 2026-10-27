[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / IAM / Service Account Key Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | Service Account Key Rotation |
| **Cloud** | GOOGLE |
| **Category** | IAM |
| **Description** | Ensures that service account keys are rotated within 90 days of creation. |
| **More Info** | Service account keys should be rotated so older keys that that might have been lost or compromised cannot be used to access Google services. |
| **GOOGLE Link** | https://cloud.google.com/iam/docs/key-rotation |
| **Recommended Action** | Rotate service account keys that have not been rotated in over 90 days. |

## Detailed Remediation Steps
1. Log in to the Google Cloud console and select the project that contains the service account.
2. Go to **IAM & Admin > Service Accounts**.
3. Select the service account, open its **Keys** tab, and identify user-managed keys whose valid-after/creation time is older than 90 days (or your approved policy threshold).
4. For each overdue key, create a replacement using **Add key > Create new key**. Store the downloaded private key only in your approved secret-management system; do not commit it or write it to logs.
5. Update every workload that uses the service account to use the replacement key, and verify that each workload authenticates and performs its expected operation while the old key remains enabled.
6. Disable the old key and monitor the affected workloads. If a workload stops working, update that remaining consumer before proceeding.
7. After confirming that no workload depends on the old key, delete it from the service account's **Keys** tab. Deletion is permanent. Repeat for each overdue key.

**Important:** Service-account key rotation replaces user-managed credentials. Do not use the **Cryptographic keys** page or its **rotation period** setting; those controls configure Cloud KMS keys and do not rotate service-account keys. See Google's [service account key rotation guidance](https://cloud.google.com/iam/docs/key-rotation) for the full procedure.

