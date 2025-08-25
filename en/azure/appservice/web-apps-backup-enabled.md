[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Services / Web Apps Backup Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Web Apps Custom Backup Enabled |
| **Cloud** | AZURE |
| **Category** | App Services |
| **Description** | Ensures that Azure Web Apps have custom automated backups enabled. |
| **More Info** | Protect your Azure App Services web applications against accidental deletion and/or corruption, you can configure application backups to create restorable copies of your app content. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/app-service/manage-backup |
| **Recommended Action** | Configure custom automated backup for Azure Web Apps.

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.

2. In the search bar at the top, select Search resources, services, and docs and search for "App Services".
</br> <img src="/resources/azure/appservice/web-apps-backup-enabled/step2.png"/>

3. In the search results for "App Services", select the web app you have created.
</br> <img src="/resources/azure/appservice/web-apps-backup-enabled/step3.png"/>

4. After selecting the web app , a left sidebar will appear. Locate the "Settings" section.Click on "Backup".
</br> <img src="/resources/azure/appservice/web-apps-backup-enabled/step4.png"/>

5. On the top click on the "Configure custom backups" and right side will appear and create new storage account and container. </br> <img src="/resources/azure/appservice/web-apps-backup-enabled/step5.png" />
