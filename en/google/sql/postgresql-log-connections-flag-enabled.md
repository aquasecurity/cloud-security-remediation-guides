[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Connections Flag Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Connections Flag Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log connections flag enabled. |
| **More Info** | SQL instance for PostgreSQL databases provides log_connections flag. It is used to log every attempt to connect to the db server. It is not enabled by default. Enabling it will make sure to log all connection tries |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log connections flag is enabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Scroll down to the Flags section.
4. To set a flag that has not been set on the instance before, click Add item, choose the flag from the drop-down menu, and set its value.
5. Click Save to save your changes.
6. Confirm your changes under Flags on the Overview page.