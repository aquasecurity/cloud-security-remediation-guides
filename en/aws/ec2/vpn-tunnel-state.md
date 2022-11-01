[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPN Tunnel State

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPN Tunnel State |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that each AWS Virtual Private Network (VPN) connection has all tunnels up. |
| **More Info** | AWS Virtual Private Network (VPN) should have tunnels up to ensure network traffic flow over Virtual Private Network. |
| **AWS Link** | https://docs.aws.amazon.com/vpn/latest/s2svpn/VPNTunnels.html |
| **Recommended Action** | Establish a successful VPN connection using IKE or IPsec configuration |

## Detailed Remediation Steps
You can modify the tunnel options for the VPN tunnels in your Site-to-Site VPN connection. You can modify one VPN tunnel at a time.
Important
When you modify a VPN tunnel, connectivity over the tunnel is interrupted for up to several minutes. Ensure that you plan for the expected downtime.

To modify the VPN tunnel options using the console </br>

1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Site-to-Site VPN Connections. </br>
3. Select the Site-to-Site VPN connection, and choose Actions, Modify VPN Tunnel Options. </br>
4. For VPN Tunnel Outside IP Address, choose the tunnel endpoint IP of the VPN tunnel that you're modifying options for. </br>
5. Choose or enter new values for the tunnel options. For more information, see https://docs.aws.amazon.com/vpn/latest/s2svpn/VPNTunnels.html. </br>
6. Choose Save. </br>

If you don't have any  tunnel configured and need to create a Site-to-Site VPN connection </br>
1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Site-to-Site VPN Connections, Create VPN connection. </br>
3. (Optional) For Name tag, enter a name for your Site-to-Site VPN connection. Doing so creates a tag with a key of Name and the value that you specify. </br>
4. For Target gateway type, choose either Virtual private gateway or Transit gateway. Then, choose the virtual private gateway or transit gateway that you created earlier. </br>
5. For Customer gateway, select Existing, then choose the customer gateway that you created earlier from the drop-down list under Customer gateway ID. </br>
6. Select one of the routing options based on whether your customer gateway device supports Border Gateway Protocol (BGP): </br>
a. If your customer gateway device supports BGP, choose Dynamic (requires BGP). </br>
b. If your customer gateway device does not support BGP, choose Static. For Static IP Prefixes, specify each IP prefix for the private network of your Site-to-Site VPN connection. </br>
7. (Optional) If your target gateway type is transit gateway, for Tunnel Inside IP Version, specify whether the VPN tunnels support IPv4 or IPv6 traffic. IPv6 traffic is only supported for VPN connections on a transit gateway. </br>
8. (Optional) If you specified IPv4 for Tunnel Inside IP Version, you can optionally specify the IPv4 CIDR ranges for the customer gateway and AWS sides that are allowed to communicate over the VPN tunnels. The default is 0.0.0.0/0. </br>
9. For Outside IP address type, leave the default option of PublicIpv4 selected. </br>
10. (Optional) For Tunnel Options, you can specify the following information for each tunnel: </br>
a. A size /30 IPv4 CIDR block from the 169.254.0.0/16 range for the inside tunnel IPv4 addresses. </br>
b. If you specified IPv6 for Tunnel Inside IP Version, a /126 IPv6 CIDR block from the fd00::/8 range for the inside tunnel IPv6 addresses. </br>
c. The IKE pre-shared key (PSK). The following versions are supported: IKEv1 or IKEv2. </br>
d. Advanced tunnel information, which includes the following: </br>
Encryption algorithms for phases 1 and 2 of the IKE negotiations </br>
Integrity algorithms for phases 1 and 2 of the IKE negotiations </br>
Diffie-Hellman groups for phases 1 and 2 of the IKE negotiations </br>
IKE version </br>
Phase 1 and 2 lifetimes </br>
Rekey margin time </br>
Rekey fuzz </br>
Replay window size </br>
Dead peer detection interval </br>
Dead peer detection timeout action </br>
Startup action </br>
VPN tunnel logging options </br>
11. Choose Create VPN connection. It might take a few minutes to create the Site-to-Site VPN connection. </br>