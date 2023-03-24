[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Checkpoints Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Checkpoints Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensure that log_checkpoints flag is enabled for PostgreSQL instances. |
| **More Info** | When log_checkpoints flag is enabled, instance checkpoints and restart points are logged in the server log. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags#setting_a_database_flag |
| **Recommended Action** | Ensure that all PostgreSQL database instances have log_checkpoints flag and it value is set to on. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `log_checkpoints` flag from the drop-down menu, and set its value to `on`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.