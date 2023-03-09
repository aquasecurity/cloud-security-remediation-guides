[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Min Duration Statement

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Min Duration Statement |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log min duration statement flag disabled. |
| **More Info** | SQL instance for PostgreSQL databases provides log_min_duration_statement flag. It is used to log the duration of every completed statement. This should always be disabled as there can be sensitive information as well that should not be recorded in the logs. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log_min_duration_statement flag is disabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `log_min_duration_statement` flag from the drop-down menu, and set its value to `-1`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.