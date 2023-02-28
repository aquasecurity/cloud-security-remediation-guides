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
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Open the Database flags section.
4. Click the X next to the "log_min_duration_statement" flag.
5. Click Save to save your changes.