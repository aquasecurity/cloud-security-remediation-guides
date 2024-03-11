[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / VPC DNS Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC DNS Logging Enabled |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Ensure that All VPC Network has DNS logging enabled. |
| **More Info** | Cloud DNS logging records the queries coming from Compute Engine VMs, GKE containers, or other GCP resources provisioned within the VPC to Stackdriver. |
| **GOOGLE Link** | https://cloud.google.com/dns/docs/monitoring |
| **Recommended Action** | Create Cloud DNS Server Policy with logging enabled for VPC Networks |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Click  Activate Cloud Shell at the top of the Google Cloud console.
    - A Cloud Shell session opens inside a new frame at the bottom of the Google Cloud console and displays a command-line prompt. It can take a few seconds for the session to be initialized.
3. To enable logging for a network that does not have a DNS policy, run the dns policies create command with the following parameters. Replace the `POLICY_NAME`, `NETWORK`, and `DESCRIPTION` variables.
```
gcloud dns policies create POLICY_NAME \
    --networks=NETWORK \
    --enable-logging \
    --description=DESCRIPTION
``` 
4. To enable logging for a network that has an existing DNS policy, run the dns policies update command witht he following parameters Replace the `POLICY_NAME`, and `NETWORK` variables.
```
gcloud dns policies update POLICY_NAME \
    --networks=NETWORK \
    --enable-logging
```
5. Repeat steps 3 or 4 for all applicable VPC networks.

**These configuration changes may incur additional costs**