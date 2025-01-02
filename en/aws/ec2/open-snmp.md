[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open SNMP

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open SNMP |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if UDP port 161 for SNMP is open to the public. |
| **More Info** | SNMP UDP 161 used by various devices and applications for logging events, monitoring and management. Allowing Inbound traffic from any external IP address on port 161 is vulnerable to DoS attack. It is a best practice to block port 161 completely unless explicitly required. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/changing-security-group.html#add-remove-security-group-rules |
| **Recommended Action** | Restrict UDP port 161 to known IP addresses. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. From "Services" menu, select "EC2". </br> <img src="/resources/aws/ec2/open-snmp/step2.png"/>
3. In the left navigation pane, under "Network & Security", click "Security Groups".</br> <img src="/resources/aws/ec2/open-snmp/step3.png"/>
4. Select the "EC2 Security Group" that needs to be updated. </br> <img src="/resources/aws/ec2/open-snmp/step4.png"/>   
5. Go to the "Inbound rules" tab and click "Edit inbound rules".</br> <img src="/resources/aws/ec2/open-snmp/step5.png"/>
6. For any inbound rule allowing unrestricted access (source set to 0.0.0.0/0 or ::/0) to port 161, take the following actions:
   * From the **Source** dropdown, select one of the following:
     * **My IP** (if you have a static IP) to restrict access to your machine only (ideal for administrative purposes).</br> <img src="/resources/aws/ec2/open-snmp/step6-1.png"/> 
     * **Custom**: specify trusted IP ranges using CIDR notation, such as:</br> <img src="/resources/aws/ec2/open-snmp/step6-2.png"/> 
       * A single IP: `203.0.113.25/32`.
       * A subnet: `203.0.113.0/24`.
       * A Security Group ID for internal AWS access.
7. Click "Save rules" to apply the updated security group settings. </br> <img src="/resources/aws/ec2/open-snmp/step7.png"/>
8. Switch AWS regions in the top navigation bar to repeat this process for other regions.
