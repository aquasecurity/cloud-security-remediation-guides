[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Public Access Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Public Access Disabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures ability to disable public access |
| **More Info** | Disabling public access allows one to ensure that information cannot be accessed by others. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/ip-addresses/reserve-static-external-ip-address |
| **Recommended Action** | Reserve a static external IP Address. |

## Detailed Remediation Steps
1.  Go to the Reserve a static address page.

    [Go to Reserve a static address](https://console.cloud.google.com/networking/addresses/add)

2.  Choose a name for the new address.

3.  Specify whether it is an `IPv4` or `IPv6` address. Global `IPv6` addresses can only be used with global load balancers.

4.  Specify whether this IP address is regional or global. If you are reserving a static IP address for an instance or for a regional load balancer, choose Regional. If you are reserving a static IP address for a global load balancer, choose Global.

5.  If this is a regional IP address, select the region to create the address in.

6.  Optional: Select a resource to attach the IP.

7.  Click Reserve to reserve the IP.