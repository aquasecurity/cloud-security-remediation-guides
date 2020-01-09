[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Table Service / Table Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Table Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | Table Service |
| **Description** | Ensures tables do not allow full write, delete, or read ACL permissions |
| **More Info** | Table Service tables can be configured to allow to read, write or delete on objects. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/tables/table-storage-quickstart-portal |
| **Recommended Action** | Disable global read, write, and delete policies on all tables and ensure the ACL is configured with least privileges. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step3.png"/>
4. Click on the "Overveiw" in the selected "Storage account" and scroll down the right side of the settings and click on the "Tables" option.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step4.png"/>
5. Select the "Table" by clicking on three dot options at the right corner to access the "Access policy." </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step5.png"/>
6. In the selected "Table",check the "Permissions" assosciated with the "Table". If the "Table" allow full write, delete, or read ACL permissions then the selected "Table" is not as per the standard configurations.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Table" in the Azure account. </br>
8. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Overview" options and select the "Table" by clicking on the dots and click on the "Access policy" to access the configurations.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step8.png"/>
9. On the "Table" configuration select the "Edit" option to make the changes.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step9.png"/>
10. Uncheck the global read/write/detele policies under the "Permissions" and click on the "OK" button to make the changes.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step10.png"/>
11. Repeat steps number 8 - 10 to ensures "Tables" do not allow full write, delete, or read ACL permissions. </br>

