[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Disk In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk In Use |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Writing and reading data from Cloud Storage buckets |
| **More Info** | Write and read files from Cloud Storage buckets by using the `gsutil` command-line tool or the Cloud Storage API. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks |
| **Recommended Action** | Read and write from storage buckets. |

## Detailed Remediation Steps
By default, the `gsutil` command-line tool is installed on most VMs that use [public images](https://cloud.google.com/compute/docs/images/os-details). If your VM doesn't have the `gsutil` command-line tool, you can [install `gsutil` as part of the Google Cloud CLI](https://cloud.google.com/storage/docs/gsutil_install).

1.  [Connect to an instance](https://cloud.google.com/compute/docs/instances/connecting-to-instance).

    a.  In the Google Cloud console, go to the VM instances page.

        [Go to VM instances](https://console.cloud.google.com/compute/instances)

    b.  In the list of virtual machine instances, click SSH in the row of the instance that you want to connect to.

2.  If you have never used `gsutil` on this instance before, use the gcloud CLI to set up credentials.

    gcloud init

    Alternatively, if your instance is configured to use a [service account](https://cloud.google.com/compute/docs/access/service-accounts) with a Cloud Storage scope, you can skip this step.

3.  Use the `gsutil` tool to [create buckets, write data to buckets, and read data from those buckets](https://cloud.google.com/storage/docs/quickstart-gsutil#create). To write or read data from a specific bucket, you must have access to the bucket. You can read data from any bucket that is publicly accessible.

    Optionally, you can also [stream data](https://cloud.google.com/storage/docs/streaming-uploads) to Cloud Storage.