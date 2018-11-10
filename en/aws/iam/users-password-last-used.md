[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Users Password Last Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | Users Password Last Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects users with password logins that have not been used for a period of time and that should be decommissioned |
| **More Info** | Having numerous, unused user accounts extends the attack surface. If users do not log into their accounts for more than the defined period of time, the account should be deleted. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_admin-change-user.html |
| **Recommended Action** | Delete old user accounts that allow password-based logins and have not been used recently. |

## Detailed Remediation Steps

