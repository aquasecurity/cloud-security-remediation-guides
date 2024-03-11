[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SQL Cross DB Ownership Chaining

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Cross DB Ownership Chaining |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL database instances of SQL Server type have cross db ownership chaining flag disabled. |
| **More Info** | SQL databases of SQL Server provide cross DB ownership chaining flag. It is used to configure cross-database ownership chaining for all databases. It is enabled by default and should be disabled for security unless all required. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/sqlserver/flags |
| **Recommended Action** | Ensure that cross DB ownership chaining flag is disabled for all SQLServer instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. Select the `cross db ownership chaining` flag and set its value to `off`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.