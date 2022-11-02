[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CodeBuild / Project Artifacts Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Project Artifacts Encrypted |
| **Cloud** | AWS |
| **Category** | CodeBuild |
| **Description** | Ensure that your AWS CodeBuild project artifacts are encrypted with desired encryption level. |
| **More Info** | AWS CodeBuild encrypts artifacts such as a cache, logs, exported raw test report data files, and build results by default using AWS managed keys. Use customer-managed key instead, in order to to gain more granular control over encryption/decryption process. |
| **AWS Link** | https://docs.aws.amazon.com/codebuild/latest/userguide/security-encryption.html |
| **Recommended Action** | Encrypt them using customer-managed keys to gain more control over data encryption and decryption process. |
## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Key Management Service".</br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step2.png"/>
3. From "Key Management Service (KMS)" on the left hand side and select "Customer managed keys".</br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step3.png"/>
4. On the Customer managed keys page there are two options:
    * Click on the Alias or the Key ID of the custom key that you would like to use and copy its ARN from the top bar. </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step4_1.png"/>
    * Press "Create Key on the top right" and create a custom key. After that is done, copy the key's ARN. </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step4_2.png"/>
5. Select the "Services" option again and search for "CodeBuild".
6. On the left hand side select "Build projects". </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step6.png"/>
7. If creating a new build project
    1. Press "create build project" on the top right.
    2. Scroll all the way down to the Artifacts section and select "Additional configuration". </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step7_2.png"/>
    3. Insert the ARN of the custom key into the "Encryption key" field. </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step7_3.png"/>
    4. Fill out the rest and press "Create build project".
8. If editing an existing build project.
    1. Click on the name of the project that needs to be edited.
    2. On the top right click "Edit" and select "Artifacts" from the drop down menu. </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step8_2.png"/>
    3. Click on "Additional configuration" and paste the ARN of the custom key into the "Encryption key" field. </br> <img src="/resources/aws/codebuild/project-artifacts-encrypted/step7_2.png"/>
    4. Press "Update artifacts".