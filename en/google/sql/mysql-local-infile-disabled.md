[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / MySQL Local Infile Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | MySQL Local Infile Disabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for MySQL type does not have local infile flag enabled. |
| **More Info** | SQL instances for MySQL type database provides local_infile flag, which can be used to load data from client or server systems. It controls the load data statements for database. Anyone using this server can access any file on the client system. For security reasons it should be disabled. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/flags |
| **Recommended Action** | Ensure that local infile flag is disabled for all MySQL instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `local_infile` flag from the drop-down menu, and set its value to `off`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.