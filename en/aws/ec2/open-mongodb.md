[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Open MongoDB

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open MongoDB |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if TCP port 27017 or 27018 or 27019 for MongoDB is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as MongoDB should be restricted to known IP addresses. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/changing-security-group.html#add-remove-security-group-rules |
| **Recommended Action** | Restrict TCP port 27017 or 27018 or 27019 to known IP addresses. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. From "Services" menu, select "EC2". </br> <img src="/resources/aws/ec2/open-mongodb/step2.png"/>
3. In the left navigation pane, under "Network & Security", click "Security Groups".</br> <img src="/resources/aws/ec2/open-mongodb/step3.png"/>
4. Select the "EC2 Security Group" that needs to be updated. </br> <img src="/resources/aws/ec2/open-mongodb/step4.png"/>   
5. Go to the "Inbound rules" tab and click "Edit inbound rules".</br> <img src="/resources/aws/ec2/open-mongodb/step5.png"/>
6. For any inbound rule allowing unrestricted access to TCP port 27017, 27018 or 27019 (source set to 0.0.0.0/0 or ::/0), take the following actions:
   * From the **Source** dropdown, select one of the following:
     * **My IP** (if you have a static IP) to restrict access to your machine only.</br> <img src="/resources/aws/ec2/open-mongodb/step6-1.png"/>
     * **Custom** and specify: </br> <img src="/resources/aws/ec2/open-mongodb/step6-2.png"/>
       * The static IP or Elastic IP of an authorized machine, using the /32 suffix (e.g., 203.0.113.25/32) for single-host access.
       * An IP address range for trusted networks in CIDR notation (e.g., 203.0.113.0/24).
       * The **Security Group ID** of another trusted group in the same region.
7. Click the "Save rules" to apply the updates. </br> <img src="/resources/aws/ec2/open-mongodb/step7.png"/>
8. Repeat steps 4 to 7 to update other EC2 security groups that permit unrestricted access to the MongoDB database.
9. Switch AWS regions in the top navigation bar to repeat this process for other regions.