[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Send Alerts Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Send Alerts Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that send alerts is enabled in advanced data security for SQL servers. |
| **More Info** | Enabling send alerts in advanced data security on all SQL servers ensures that monitored data for unusual activity, vulnerabilities, and threats get sent to the email addresses configured in advanced data protections. |
| **AZURE Link** | https://docs.microsoft.com/en-gb/azure/sql-database/sql-database-advanced-data-security |
| **Recommended Action** | Ensure that an email address is activated under send alerts in advanced data security for all SQL servers. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Microsoft defender for cloud" under "Security".</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step4.png"/>
5. On the "Microsoft defender for cloud" page, click on "Configure" next to "Microsoft Defender for SQL". </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step5.png"/>
6. On the "Server settings" page, scroll down to "ADVANCED THREAT PROTECTION SETTINGS" and click on "Add your contact details to the subscription's email settings in Defender for Cloud".</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step6.png"/>
7. On the "Email notifications" page if there is no email address configured and no roles are selected then send alerts are not enabled.</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step7.png"/>
8. To enable send alerts, under "Email receipients" select "Owner", "AccountAdmin". ServiceAdmin" from the dropdown and assign an email for "Additional emal addresses". </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step8.png"/>
9. In the "Notification types" checkmark "Notify about alerts with the following severity (or higher)" and selectv "High" from the dropdown.</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step9.png"/>
10. Click "Save" at the top to make the necessary changes.</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step9.png"/>
11. Repeat steps 3-10 to ensure that an email address is activated under send alerts for all SQL servers.
