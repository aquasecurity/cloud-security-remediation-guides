[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Unused VPC Internet Gateways

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unused VPC Internet Gateways |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that unused VPC Internet Gateways and Egress-Only Internet Gateways are removed |
| **More Info** | Unused VPC Internet Gateways and Egress-Only Internet Gateways must be removed to avoid reaching the internet gateway limit |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html |
| **Recommended Action** | Remove the unused/detached Internet Gateways and Egress-Only Internet Gateways |

## Detailed Remediation Steps
To detach an internet gateway </br>
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for VPC. </br> 
3. In the navigation pane, choose Elastic IPs and select the Elastic IP address. </br>
4. Choose Actions, Disassociate address. Choose Disassociate address. </br>
5. In the navigation pane, choose Internet gateways. </br>
6. Select the internet gateway and choose Actions, Detach from VPC. </br>
7. In the Detach from VPC dialog box, choose Detach internet gateway. </br>

To delete an internet gateway </br>
1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Internet gateways. </br>
3. Select the internet gateway and choose Actions, Delete internet gateway. </br>
4. In the Delete internet gateway dialog box, enter delete, and choose Delete internet gateway. </br>