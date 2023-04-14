[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Default Service Account
## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Default Service Account |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that compute instances are not configured to use the default service account. |
| **More Info** | Default service account has the editor role permissions. Due to security reasons it should not be used for any instance. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/access/service-accounts |
| **Recommended Action** | Make sure that compute instances are not using default service account |

## Detailed Remediation Steps
1. In the Google Cloud Console, go to the [VM instances](#https://console.cloud.google.com/compute/instances?_ga=2.18084025.1677574654.1681411030-795998208.1675186198) page.

2. Click the VM instance name for which you want to change the service account.

3. If the instance is not stopped, click Stop. Wait for the instance to be stopped.

4. Next, click Edit.

5. Scroll down to the Service Account section.

6. From the drop-down list, select the service account to assign to the instance.

    - Choose a service account other than the default. The VM's access scope defaults to the cloud-platform scope. You can modify the scope by using the gcloud CLI or Compute Engine API.
    - For more information about setting access scopes, see [Best practices](#https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances#best_practices).

7. Click Save to save your changes.