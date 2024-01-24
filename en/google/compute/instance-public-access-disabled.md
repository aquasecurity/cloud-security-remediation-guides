[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Public Access Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Public Access Disabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that compute instances are not configured to allow public access. |
| **More Info** | Compute Instances should always be configured behind load balancers instead of having public IP addresses in order to minimize the instance\'s exposure to the internet. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/ip-addresses/reserve-static-external-ip-address |
| **Recommended Action** | Modify compute instances and set External IP to None for network interface. |

## Detailed Remediation Steps
1. Log in to the [GCP Console](https://console.cloud.google.com). </br>
2. Navigate to VM instances.</br><img src="/resources/google/compute/instance-public-access-disabled/step2.png"/></br>
3. In the Instance detail page, click the instance name.</br>
4. Click Edit.</br><img src="/resources/google/compute/instance-public-access-disabled/step4.png"/></br>
5. For each Network interface, ensure that External IP is set to None.</br><img src="/resources/google/compute/instance-public-access-disabled/step5.png"/></br>
6. Click Done, then click Save.</br>
