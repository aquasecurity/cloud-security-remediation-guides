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
### Name

gcloud dataflow jobs cancel - cancels all jobs that match the command line arguments

### Synopsis

`gcloud dataflow jobs cancel` `*[JOB_ID](https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel#JOB_ID)*` [`*[JOB_ID](https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel#JOB_ID)*` ...] [`[--force](https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel#--force)`] [`[--region](https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel#--region)`=`*REGION_ID*`] [`*[GCLOUD_WIDE_FLAG](https://cloud.google.com/sdk/gcloud/reference/dataflow/jobs/cancel#GCLOUD-WIDE-FLAGS) ...*`]

### Flags

`--force`

Forcibly cancels a Dataflow job, leaking any VMs the Dataflow job created. Regular cancel must have been attempted at least 30 minutes ago for a job to be force cancelled.

`--region`=`*REGION_ID*`

The region ID of the jobs' regional endpoint. Defaults to 'us-central1'.

### GCloud Wide Flags

These flags are available to all commands: `[--access-token-file](https://cloud.google.com/sdk/gcloud/reference#--access-token-file)`, `[--account](https://cloud.google.com/sdk/gcloud/reference#--account)`, `[--billing-project](https://cloud.google.com/sdk/gcloud/reference#--billing-project)`, `[--configuration](https://cloud.google.com/sdk/gcloud/reference#--configuration)`, `[--flags-file](https://cloud.google.com/sdk/gcloud/reference#--flags-file)`, `[--flatten](https://cloud.google.com/sdk/gcloud/reference#--flatten)`, `[--format](https://cloud.google.com/sdk/gcloud/reference#--format)`, `[--help](https://cloud.google.com/sdk/gcloud/reference#--help)`, `[--impersonate-service-account](https://cloud.google.com/sdk/gcloud/reference#--impersonate-service-account)`, `[--log-http](https://cloud.google.com/sdk/gcloud/reference#--log-http)`, `[--project](https://cloud.google.com/sdk/gcloud/reference#--project)`, `[--quiet](https://cloud.google.com/sdk/gcloud/reference#--quiet)`, `[--trace-token](https://cloud.google.com/sdk/gcloud/reference#--trace-token)`, `[--user-output-enabled](https://cloud.google.com/sdk/gcloud/reference#--user-output-enabled)`, `[--verbosity](https://cloud.google.com/sdk/gcloud/reference#--verbosity)`.

Run `$ [gcloud help](https://cloud.google.com/sdk/gcloud/reference)` for details.

### Notes

This variant is also available:

```
gcloud beta dataflow jobs cancel
```