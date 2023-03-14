[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Shielded VM Enabled
## Quick Info

| | |
|-|-|
| **Plugin Title** | Shielded VM Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that instances are configured with the shielded VM enabled |
| **More Info** | Shielded VM option should be configured to defend against the security attacks on the instances. |
| **GOOGLE Link** | https://cloud.google.com/security/shielded-cloud/shielded-vm |
| **Recommended Action** | Enable the shielded VM for all the instances for security reasons. |

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the VM instances page.

    [Go to VM instances](https://console.cloud.google.com/compute/instances)

2.  Click the instance name to open the VM instance details page.

3.  Click Stop.

4.  After the instance stops, click Edit.

5.  In the Shielded VM section, modify the Shielded VM options:

    -   Toggle Turn on Secure Boot to enable Secure Boot Compute Engine does not enable [Secure Boot](https://cloud.google.com/compute/shielded-vm/docs/shielded-vm#secure-boot) by default because unsigned drivers and other low-level software might not be compatible. If possible, Google recommends enabling Secure Boot.

    -   Toggle Turn on vTPM to disable the virtual trusted platform module (vTPM). By default, Compute Engine enables the [Virtual Trusted Platform Module (vTPM)](https://cloud.google.com/compute/shielded-vm/docs/shielded-vm#vtpm).

    -   Toggle Turn on Integrity Monitoring to disable integrity monitoring. By default, Compute Engine enables [integrity monitoring](https://cloud.google.com/compute/shielded-vm/docs/shielded-vm#integrity-monitoring).

6.  Click Save.

7.  Click Start to start the instance.