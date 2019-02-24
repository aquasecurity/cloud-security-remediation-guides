[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SSM / SSM Encrypted Parameters

## Quick Info

| | |
|-|-|
| **Plugin Title** | SSM Encrypted Parameters |
| **Cloud** | AWS |
| **Category** | SSM |
| **Description** | Ensures SSM Parameters are encrypted |
| **More Info** | SSM Parameters should be encrypted. This allows their values to be used by approved systems, while restricting access to other users of the account. |
| **AWS Link** | https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-paramstore-about.html#sysman-paramstore-securestring |
| **Recommended Action** | Recreate unencrypted SSM Parameters with Type set to SecureString. |

## Detailed Remediation Steps

