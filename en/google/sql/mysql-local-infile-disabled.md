[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / MySQL Local Infile Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | MySQL Local Infile Disabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances for MySQL type does not have local infile flag enabled. |
| **More Info** | SQL instances for MySQL type database provides local_infile flag, which can be used to load data from client or server systems. It controls the load data statements for database. Anyone using this server can access any file on the client system. For security reasons it should be disabled. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/flags |
| **Recommended Action** | Ensure that local infile flag is disabled for all MySQL instances. |

## Detailed Remediation Steps
1. In the Google Cloud console, create a new Google Cloud console project, or open an existing project by selecting the project name.
2. Open the instance and click Edit.
3. Scroll down to the Flags section.
4. To set a flag that has not been set on the instance before, click Add item, choose the flag from the drop-down menu, and set its value.
5. Click Save to save your changes.
6. Confirm your changes under Flags on the Overview page.