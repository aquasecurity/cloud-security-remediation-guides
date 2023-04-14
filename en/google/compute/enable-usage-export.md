[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Enable Usage Export

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enable Usage Export |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that setting is configured to export Compute instances usage to Cloud Storage bucket. |
| **More Info** | Compute Engine lets you export detailed reports that provide information about the lifetime and usage of your Compute Engine resources to a Google Cloud Storage bucket using the usage export feature. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/logging/usage-export |
| **Recommended Action** | Ensure that Enable Usage Export setting is configured for your GCP project. |

## Detailed Remediation Steps
1. Sign in to the Google Cloud Console, and go to the [Compute Engine Settings](#https://console.cloud.google.com/compute/settings?_ga=2.223580315.1677574654.1681411030-795998208.1675186198) page.

2. Check the Enable usage export box.

3. Fill in the field asking for a Bucket name. Optionally, provide a Report prefix, if desired. If you leave the report prefix empty, the default prefix usage_gce is used. All usage reports delivered to the bucket are named with this prefix.

4. Click Save.