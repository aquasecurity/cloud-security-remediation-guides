[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Dataflow / Dataflow Hanged Jobs
## Quick Info

| | |
|-|-|
| **Plugin Title** | Dataflow Hanged Jobs |
| **Cloud** | GOOGLE |
| **Category** | Datflow |
| **Description** | Ensure that Cloud Dataflow jobs are not in same state for more than defined amount of time. |
| **More Info** | Cloud Dataflow jobs transit between different states and normally reach terminal state. If they stay in same state for abnormal amount of time, job administrator should stop such jobs to save unnecessary cost. |
| **GOOGLE Link** | https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel |
| **Recommended Action** | Cancel/stop Dataflow jobs which are in same state for more than set amount of time. |

## Detailed Remediation Steps
1. The 'gcloud dataflow jobs cancel' commandlet cancels all jobs that match the command line arguments.

2. To cancel jobs, log into the Google Cloud Console and open a cloud shell instance. See [Using Cloud Shell](#https://cloud.google.com/shell/docs/using-cloud-shell) for more details on access.

3. Run the command in the following manner, replacing the variables with values corresponding to your organization:
  ```
  gcloud dataflow jobs cancel JOB_ID [JOB_ID …] [--force] [--region=REGION_ID] [GCLOUD_WIDE_FLAG …]
  ```

4. This variant is also available:
  ```
  gcloud beta dataflow jobs cancel
  ```
