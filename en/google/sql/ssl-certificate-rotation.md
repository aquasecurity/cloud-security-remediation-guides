[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / SSL Certificate Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | SSL Certificate Rotation |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensure that server certificates configured for Cloud SQL are rotated before they expire. |
| **More Info** | Server certificates configured for Cloud SQL DB instances should be rotated before they expire to ensure that incoming connections for database instance remain secure. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/postgres/configure-ssl-instance?authuser=1#server-certs |
| **Recommended Action** | Edit Cloud SQL DB instances and rotate server certificates under Connections->MANAGE CERTIFICATES |

## Detailed Remediation Steps
1. In the Google Cloud console, go to the [Cloud SQL Instances](https://console.cloud.google.com/sql?authuser=1&_ga=2.184743081.1679736441.1679922535-795998208.1675186198) page.
2. Go to Cloud SQL Instances
3. To open the Overview page of an instance, click the instance name.
4. Click Connections from the SQL navigation menu.
5. Select the Security tab.
6. Scroll down to the Manage server certificates section. You can see the expiration date of your server certificate in the table.
7. Select Rotate certificate. The rotate option will be grayed-out if there are no eligible certificates.
8. Click Download Certificates.
    The server certificate information, encoded as a PEM file, is downloaded to your local environment:

    Update all of your PostgreSQL clients to use the new information by copying the downloaded file to your client host machines, replacing the existing server-ca.pem file.
9. After you have updated your clients, continue to complete the rotation.
10. Return to the Security tab.
11. Click to expand Manage certificates.
12. Select Rotate certificate.
13. Confirm that your clients are connecting properly.
    If any clients are not connecting using the newly rotated certificate, you can select Rollback certificate to rollback to the previous configuration.