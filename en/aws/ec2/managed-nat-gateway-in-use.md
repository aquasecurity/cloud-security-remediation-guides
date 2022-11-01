[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Managed NAT Gateway In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Managed NAT Gateway In Use |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure AWS VPC Managed NAT (Network Address Translation) Gateway service is enabled for high availability (HA) |
| **More Info** | VPCs should use highly available Managed NAT Gateways in order to enable EC2 instances to connect to the internet or with other AWS components |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html |
| **Recommended Action** | Update VPCs to use Managed NAT Gateways instead of NAT instances |

## Detailed Remediation Steps
Creating a Managed NAT Gateway </br>
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for VPC. </br> 
3. At the navigation area on the left. Locate and click on NAT Gateways: </br>
4. Then click on Create NAT Gateway and choose one of your subnets. </br>
5. Choose one of your existing Elastic IP addresses, or create a new one. </br>
6. Then click on Create a NAT Gateway, and observe the confirmation. </br>
7. you will need to edit your VPC’s route tables to send traffic destined for the Internet toward the gateway. The gateway’s internal (private) IP address will be chosen automatically, and will be on the subnet associated with the gateway.  </br>