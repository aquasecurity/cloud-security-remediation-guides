[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Disconnections Flag Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Disconnections Flag Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log disconnections flag enabled. |
| **More Info** | SQL instance for PostgreSQL databases provides log_disconnections flag. It is used to log every attempt to connect to the DB server. It is not enabled by default. Enabling it will make sure to log anyone who disconnects from the instance. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log disconnections flag is enabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL".
3. On the "SQL" page, select the SQL Instance which needs to be verified whether it has flags added or not by opening the instance and clicking Edit.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `log_disconnections` flag from the drop-down menu, and set its value to On.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.