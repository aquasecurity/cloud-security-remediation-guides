[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / File Storage / NFS Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | NFS Public Access |
| **Cloud** | ORACLE |
| **Category** | File Storage |
| **Description** | Ensures that all File Systems do not have public access. |
| **More Info** | All Network File Systems should be configured to only allow access from trusted sources. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/File/Tasks/exportoptions.htm |
| **Recommended Action** | 1. Enter the File Storage service. 2. Enter the File System service 3. Select the File System. 4. Select the export. 5. Ensure that the source is not 0.0.0.0/0, if so edit the NFS Export Options to not allow public access. |

## Detailed Remediation Steps

