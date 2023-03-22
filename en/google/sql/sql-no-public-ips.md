[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SQL No Public IPs

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL No Public IPs |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensure that SQL instances are using private IPs instead of public IPs. |
| **More Info** | Cloud SQL databases should always use private IP addresses which provide improved network security and lower latency. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/configure-private-ip |
| **Recommended Action** | Make sure that SQL databases IP addresses setting does not have IP address of PRIMARY type |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Select Connections from the SQL navigation menu.
5. Select the Private IP checkbox.
6. Select the VPC network you want to use.
7. If you see Private service connection required, click Set up connection.
8. Allocate an IP range section and click Continue.
9. Click Create connection.
10. Verify that you see the Private service connection for network VPC_NETWORK_NAME has been successfully created status. Click Save.