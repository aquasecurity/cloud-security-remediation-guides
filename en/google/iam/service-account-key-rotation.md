[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / IAM / Service Account Key Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | Service Account Key Rotation |
| **Cloud** | GOOGLE |
| **Category** | IAM |
| **Description** | Ensures that service account keys are rotated within 90 days of creation. |
| **More Info** | Service account keys should be rotated so older keys that that might have been lost or compromised cannot be used to access Google services. |
| **GOOGLE Link** | https://cloud.google.com/iam/docs/creating-managing-service-account-keys |
| **Recommended Action** | Rotate service account keys that have not been rotated in over 90 days. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Service accounts" option under the "IAM & Admin."</br> <img src="/resources/google/iam/service-account-key-rotation/step2.png"/>
3. On the "Service accounts" page, select the servcie account with the keys.</br> <img src="/resources/google/iam/service-account-key-rotation/step3.png"/>
4. Click on the "Cryptographic keys" on the left navigation panel under the "IAM & admin."</br> <img src="/resources/google/iam/service-account-key-rotation/step4.png"/>
5. On the "Cryptographic keys" page, click on the "Name" as a link to access the key.</br> <img src="/resources/google/iam/service-account-key-rotation/step5.png"/>
6. On the "Cryptographic keys - Edit" page, check the "Next rotation" date and if it's more than 90 days then it's not as per the best practices.</br> <img src="/resources/google/iam/service-account-key-rotation/step6.png"/>
7. Repeat steps number 2 - 6 to verify other keys in the account.</br>
8. Navigate to the "IAM & admin" on the left navigation panel, select the "Cryptographic keys" option and select the cryptographic key in the question.</br> <img src="/resources/google/iam/service-account-key-rotation/step8.png"/>
9. Click on the 3 dots at the extreme right to choose the "Edit rotation period" option to change the rotation period to 90 days.</br> <img src="/resources/google/iam/service-account-key-rotation/step9.png"/>
10. On the "Edit rotation period" tab, select the "90 days" option from the dropdown menu and click on the "Save" option to make the changes.</br> <img src="/resources/google/iam/service-account-key-rotation/step10.png"/>
11. Repeat steps number 8 - 10 to rotate service account keys that have not been rotated in over 90 days.</br>

