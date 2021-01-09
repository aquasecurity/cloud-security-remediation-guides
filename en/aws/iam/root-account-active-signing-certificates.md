[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root Account Active Signing Certificates

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root Account Active Signing Certificates |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the root user is not using x509 signing certificates |
| **More Info** | AWS supports using x509 signing certificates for API access, but these should not be attached to the root user, which has full access to the account. |
| **AWS Link** | https://docs.aws.amazon.com/whitepapers/latest/aws-overview-security-processes/x.509-certificates.html |
| **Recommended Action** | Delete the x509 certificates associated with the root account. |

## Detailed Remediation Steps




