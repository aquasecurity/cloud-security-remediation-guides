[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Automatic Restart Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Automatic Restart Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that Virtual Machine instances have automatic restart feature enabled. |
| **More Info** | Automatic Restart sets the virtual machine restart behavior when an instance is crashed or stopped by the system. If it is enabled, Google Cloud Compute Engine restarts the instance if it crashes or is stopped. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/setting-instance-scheduling-options#autorestart |
| **Recommended Action** | Ensure automatic restart is enabled for all virtual machine instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, go to the VM instances page.
2. Click the VM for which you want to change settings. The VM details page displays.
3. On the VM details page, complete the following steps:
	a. Click the Edit button at the top of the page.
	b. Under Availability policies, update the policy as needed. From the Availability policies section, you can set the On host maintenance and Automatic restart options.
	c. Click Save.
