[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Unrestricted Network ACL Outbound Traffic

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unrestricted Network ACL Outbound Traffic |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that no Amazon Network ACL allows outbound/egress traffic to all ports |
| **More Info** | Amazon Network ACL should not allow outbound/egress traffic to all ports to avoid unauthorized access at the subnet level |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html |
| **Recommended Action** | Update Network ACL to allow outbound/egress traffic to specific port ranges only |

## Detailed Remediation Steps
To delete a rule from a network ACL
1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Network ACLs, and then select the network ACL. </br>
3. In the details pane, select Outbound Rules tab, and then choose Edit. Choose Remove for the rule that allow outbound traffic to all ports, and then choose Save. </br>

Then you may add new rules to allow outbound traffic to specific port ranges as needed </br>
To add rules to a network ACL: </br>
1. Open the Amazon VPC console at https://console.aws.amazon.com/vpc/. </br>
2. In the navigation pane, choose Network ACLs. </br>
3. In the details pane, choose the Outbound Rules tab, and then choose Edit.
4. In Rule #, enter a rule number (for example, 100). The rule number must not already be in use in the network ACL. We process the rules in order, starting with the lowest number. </br>
5. Select a rule from the Type list. For example, to add a rule for HTTP, choose HTTP. To add a rule to allow all TCP traffic, choose All TCP. For some of these options (for example, HTTP), the port filled automatically. To use a protocol that's not listed, choose Custom Protocol Rule. </br>
6. (Optional) If you're creating a custom protocol rule, select the protocol's number and name from the Protocol list. </br>
7. (Optional) If the protocol you selected requires a port number, enter the port number or port range separated by a hyphen (for example, 49152-65535). </br>
8. In the Destination field, enter the CIDR range that the rule applies to. </br>
9. From the Allow/Deny list, select ALLOW to allow the specified traffic or DENY to deny the specified traffic. </br>
10. (Optional) To add another rule, choose Add another rule, and repeat steps 4 to 9 as required. </br>
11. When you are done, choose Save. </br>