[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SQL Contained Database Authentication

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Contained Database Authentication |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances of SQL Server type have Contained Database Authentication flag disabled. |
| **More Info** | Enabling Contained Database Authentication flag allows users to connect to the database without authenticating a login at the Database Engine level along with other security threats. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/sqlserver/flags |
| **Recommended Action** | Ensure that Contained Database Authentication flag is disabled for all SQL Server instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `Contained Database Authentication` flag from the drop-down menu, and set its value to `off`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.