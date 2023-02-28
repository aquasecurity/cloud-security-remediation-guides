[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / PostgreSQL Log Lock Waits Flag Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Log Lock Waits Flag Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for PostgreSQL type have log_lock_waits flag enabled. |
| **More Info** | SQL instance for PostgreSQL database provides log_lock_waits flag. It is not enabled by default. Enabling it will make sure that log messages are generated whenever a session waits longer than deadlock_timeout to acquire a lock. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/flags#config |
| **Recommended Action** | Ensure that log_lock_waits flag is enabled for all PostgreSQL instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Scroll down to the Flags section.
4. To set a flag that has not been set on the instance before, click Add item, choose the "log_lock_waits" flag from the drop-down menu, and set its value.
5. Click Save to save your changes.
6. Confirm your changes under Flags on the Overview page.