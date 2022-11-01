[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Unused Virtual Private Gateway

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unused Virtual Private Gateway |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that unused Virtual Private Gateways (VGWs) are removed. |
| **More Info** | Unused VGWs should be remove to follow best practices and to avoid reaching the service limit. |
| **AWS Link** | https://docs.aws.amazon.com/vpn/latest/s2svpn/delete-vpn.html |
| **Recommended Action** | Remove the unused Virtual Private Gateways (VGWs) |

## Detailed Remediation Steps
To detach a virtual private gateway using the console </br>
1. In the navigation pane, choose Virtual Private Gateways. </br>
2. Select the virtual private gateway and choose Actions, Detach from VPC. </br>
3. Choose Yes, Detach. </br>

If you no longer require a detached virtual private gateway, you can delete it. You can't delete a virtual private gateway that's still attached to a VPC. detach it first as mentioned in the above steps. </br>
To delete a virtual private gateway using the console </br>
1. In the navigation pane, choose Virtual Private Gateways. </br>
2. Select the virtual private gateway to delete and choose Actions, Delete Virtual Private Gateway. </br>