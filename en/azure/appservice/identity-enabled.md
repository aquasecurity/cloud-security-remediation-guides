[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Identity Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Identity Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures a system or user assigned managed identity is enabled to authenticate to App Service without storing credentials in the code. |
| **More Info** | Managing credentials in your code for authenticating to cloud services is a challenge, and maintaining the credentials secure is very important. Ideally, the credentials never appear on developer workstations and aren't checked into source control. The managed identities for Azure resources provides Azure services with an automatically managed identity in Azure AD. You can use the identity to authenticate to any service that supports Azure AD authentication, without having to include any credentials in your code. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-managed-identity |
| **Recommended Action** | In your App Service go to Identity > System assigned and set it to "On" (Enabled) or go to the User assigned tab and add a user assigned managed identity. |

## Detailed Remediation Steps

