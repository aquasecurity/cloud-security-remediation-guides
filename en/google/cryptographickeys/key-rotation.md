[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Cryptographic Keys / Key Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Rotation |
| **Cloud** | GOOGLE |
| **Category** | Cryptographic Keys |
| **Description** | Ensures cryptographic keys are set to rotate on a regular schedule |
| **More Info** | All cryptographic keys should have key rotation enabled. Google will handle the rotation of the encryption key itself, as well as storage of previous keys, so previous data does not need to be re-encrypted before the rotation occurs. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-cryptoKeys |
| **Recommended Action** | Ensure that cryptographic keys are set to rotate. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and select the "Cryptographic keys" option under the "Security."</br> <img src="/resources/google/cryptographickeys/key-rotation/step2.png"/>
3. On the "Cryptographic keys" page, select the "Name" as a link option to access the key.</br> <img src="/resources/google/cryptographickeys/key-rotation/step3.png"/>
4. On the "Cryptographic keys- Edit" page, check whether the cryptographic keys are set to rotate on a regular schedule or not.</br> <img src="/resources/google/cryptographickeys/key-rotation/step4.png"/>
5. Repeat steps number 2 - 4 to check the other cryptographic keys in the account.</br>
6. Navigate to the "Security" on the left navigation panel, select the "Cryptographic keys" option and select the cryptographic key in the question.</br> <img src="/resources/google/cryptographickeys/key-rotation/step6.png"/>
7. Click on the 3 dots at the extreme right to choose the "Edit rotation period" option to change the rotation period to 90 days and click on the "Save" button to make the changes.</br> <img src="/resources/google/cryptographickeys/key-rotation/step7.png"/>
8. Repeat steps number 6 - 7 to ensure that cryptographic keys are set to rotate.</br>
