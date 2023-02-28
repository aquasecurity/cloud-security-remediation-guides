[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Min Error Statement

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Min Error Statement |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log min error statement flag set to Error. |
| **More Info** | SQL instance for PostgreSQL databases provides log_min_error_statement flag. It is used to mention/tag that the error messages. Setting it to Error value will help to find the error messages appropriately. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log_min_error_statement flag is set to Error for all PostgreSQL instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Scroll down to the Flags section.
4. To set a flag that has not been set on the instance before, click Add item, choose the "log_min_error_statement" flag from the drop-down menu, and set its value.
5. Click Save to save your changes.
6. Confirm your changes under Flags on the Overview page.