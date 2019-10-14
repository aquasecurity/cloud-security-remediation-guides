[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Identity Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Identity Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures a system or user assigned managed identity is enabled to authenticate to App Services without storing credentials in the code. |
| **More Info** | Maintaining cloud connection credentials in code is a security risk. Credentials should never appear on developer workstations and should not be checked into source control. Managed identities for Azure resources provides Azure services with a managed identity in Azure AD which can be used to authenticate to any service that supports Azure AD authentication, without having to include any credentials in code. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-managed-identity |
| **Recommended Action** | Enable system or user-assigned identities for all App Services and avoid storing credentials in code. |

## Detailed Remediation Steps

