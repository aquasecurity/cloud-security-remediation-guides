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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step3.png"/>
4. In the left navigation panel, click on the "Tables" under "Data Storage".</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step4.png"/>
5. Select the "Table" by clicking on three dot options at the right corner to chose the "Access policy." </br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step5.png"/>
6. On the Access Policy panel on the right, check the "Permissions" assosciated with the "Table". If the "Table" allows full read, write, delete and update permissions then the selected "Table" is not as per the standard configuration.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step6.png"/>
7. To ensure tables do not allow full read, write, delete and update ACL permissions, click on the triple dot (...) at the extreme right and select "Edit".</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step7.png"/>
8. In the "Edit policy" popup uncheck the desired permissions and click on "OK" button.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step8.png"/>
9. Click on "Save" buttton at the top to make the necessary changes.</br> <img src="/resources/azure/tableservice/table-service-all-access-acl/step9.png"/>
10. Repeat steps 3 - 9 for all other tables.
