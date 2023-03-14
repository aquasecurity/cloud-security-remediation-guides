[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Maintenance Behavior

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Maintenance Behavior |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that \"On Host Maintenance\" configuration is set to Migrate for VM instances. |
| **More Info** | When Google Compute Engine performs regular maintenance of its infrastructure, it migrates your VM instances to other hardware if you have configured the availability policy for the instance to use live migration. This prevents your applications from experiencing disruptions during these events. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/setting-instance-scheduling-options |
| **Recommended Action** | Ensure that your Google Compute Engine VM instances are configured to use live migration. |

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the VM instances page.

    [Go to VM instances](https://console.cloud.google.com/compute/instances)

2.  Click the VM for which you want to change settings. The VM details page displays.

3.  On the VM details page, complete the following steps:

    1.  Click the Edit button at the top of the page.
    2.  Under Availability policies, update the policy as needed. From the Availability policies section, you can set the On host maintenance and Automatic restart options.
    3.  Click Save.