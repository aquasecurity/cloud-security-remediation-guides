[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / MySQL Slow Query Log Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | MySQL Slow Query Log Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures that MySQL instances have slow query log flag enabled. |
| **More Info** | MySQL instance flag that helps find inefficient or time-consuming SQL queries for MySQL databases. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/flags |
| **Recommended Action** | Ensure that slow query log flag is enabled for all MySQL instances. |

## Detailed Remediation Steps
1. 1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". 
3. On the "SQL" page, select the SQL Instance which needs to be verified by clicking on the checkbox next to its name.
4. Scroll down to the Flags section.
5. To set a flag that has not been set on the instance before, click Add item, choose the `slow_query_log` flag from the drop-down menu, and set its value to `on`.
6. Click Save to save your changes.
7. Confirm your changes under Flags on the Overview page.