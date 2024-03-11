[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Parser Stats Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Parser Stats Disabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log parser stats flag set to "off". |
| **More Info** | Logging parser performance stats can substantially raise the volume of logs and result in performance overhead. To prevent any performance issues caused by excessive logging, it is recommended that the "log_parser_stats" flag is set to off. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log_parser_stats flag is disabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and click on "SQL". </br> <img src="/resources/google/sql/postgresql-log-parser-stats/step2.png">
3. On the "SQL" page, click on the three dots next to the name of the PostgreSQL Instance which needs to be verified whether it has the log_parser_stats flag enabled or not and click on "Edit".</br> <img src="/resources/google/sql/postgresql-log-parser-stats/step3.png"/>
4. On the "Edit" instance page, scroll down and click on the arrow next to the "Flags" section and check if the log_parser_stats flag is set to "on". If the value is not set, the PostgreSQL instance has the log_parser_stats flag disabled. </br> <img src="/resources/google/sql/postgresql-log-parser-stats/step4.png"/>
5. Repeat steps number 3-4 to check other PostgreSQL Instances in the project.</br>
6. Navigate to "SQL" and click on it. Click on the three dots next to the name of the PostgreSQL Instance which has log_parser_stats flag enabled and click "Edit".</br> <img src="/resources/google/sql/postgresql-log-parser-stats/step3.png"/>
7. On the Edit Instance page, scroll down to the Flags section, expand it and set the value for log_parser_stats flag to "off" or click on the trash icon to remove it altogether. Then click "Save".</br> <img src="/resources/google/sql/postgresql-log-parser-stats/step7.png"/>
8. Repeat steps number 7-8 to disable log_parser_stats flag for all other PostgreSQL Instances in the project.</br>
