[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EKS / EKS Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EKS Logging Enabled |
| **Cloud** | AWS |
| **Category** | EKS |
| **Description** | Ensures all EKS cluster logs are being sent to CloudWatch |
| **More Info** | EKS supports routing of cluster event and audit logs to CloudWatch, including control plane logs. All logs should be sent to CloudWatch for security analysis. |
| **AWS Link** | https://docs.aws.amazon.com/eks/latest/userguide/control-plane-logs.html |
| **Recommended Action** | Enable all EKS cluster logs to be sent to CloudWatch with proper log retention limits. |

## Detailed Remediation Steps
1. Log into the AWS Management Console. </br>
2. Navigate to the EKS page. </br>
3. In the navigation pane click on clusters. </br>
4. Click the cluster name you need to enable logging for. </br>
5. Click on logging tab. </br>
6. Click on Manage logging. </br>
7. Enable logs for the all cluster logs: API serverLogs, AuditLogs, AuthenticatorLogs, Controller managerLogs , SchedulerLogs. </br>
8. Click save. </br>



