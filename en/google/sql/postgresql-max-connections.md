[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Max Connections

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Max Connections |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensure that max_connections is configured with optimal value for PostgreSQL instances. |
| **More Info** | An optimal value should be set for max_connections (maximum number of client connections) to meet the database workload requirements. If this no value is set for max_connections flag, instance assumes default value which is calculated per instance memory size. |
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