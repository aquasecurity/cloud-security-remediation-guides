[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Temp Files

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Temp Files |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log temp files flag enabled. |
| **More Info** | SQL instance for PostgreSQL databases provides log_temp_files flag. It is used to log the temporary files name and size. It is not enabled by default. Enabling it will make sure to log names and sizes of all the temporary files that were created during any operation(sort, hashes, query_results etc). |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags |
| **Recommended Action** | Ensure that log_temp_files flag is enabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Scroll down to the Flags section.
4. To set a flag that has not been set on the instance before, click Add item, choose the "log_temp_files" flag from the drop-down menu, and set its value.
5. Click Save to save your changes.
6. Confirm your changes under Flags on the Overview page.