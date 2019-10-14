[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Connection Throttling Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Connection Throttling Enabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures connection throttling is enabled for PostgreSQL servers |
| **More Info** | Connection throttling slows the amount of query and error logs sent by the server from the same IP address, limiting DoS attacks or the slowing down of servers due to excessive legitimate user logs. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/howto-configure-server-parameters-using-portal |
| **Recommended Action** | Ensure the server parameters for each PostgreSQL server have the connection_throttling setting enabled. |

## Detailed Remediation Steps

