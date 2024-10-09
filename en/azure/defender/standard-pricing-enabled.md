[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Standard Pricing Enabled

## Quick Info

| | |
|-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Standard Pricing Enabled |
| **Cloud** | AZURE |
| **Category** | Defender |
| **Description** | Ensures that standard pricing is enabled in Microsoft Defender for Cloud |
| **More Info** | Enabling standard pricing increases the security posture of the subscription. This enables advanced security monitoring for the services covered under Microsoft Defender for Cloud. |
| **AZURE Link** | https://azure.microsoft.com/en-us/pricing/details/defender-for-cloud/ |
| **Recommended Action** | Ensure that standard pricing is enabled in Microsoft Defender for Cloud. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/defender/standard-pricing-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down and select the "Environment Settings" option under "Management" in the left navigation panel. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step3.png"/>
4. On the "Environment Settings" page, click on the name of the Azure subscription that needs to be examined. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step4.png"/>
5. In the navigation panel, choose **Defender plans**. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step5.png"/>
6. Check the pricing tier enabled for the selected plans, ensuring that the Standard pricing tier is enabled. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step6.png"/>
7. If the **Standard Pricing** is not enabled, enable the **Standard** pricing tier for the chosen plans by selecting it. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step7.png"/>
8. Save the changes made to the selected plans at the top of the **Defender plans** page. </br> <img src="/resources/azure/defender/standard-pricing-enabled/step8.png"/>
9. Repeat steps 1-8 to verify that **Standard Pricing** is enabled across all required subscriptions.
10. Ensure that **Standard Pricing** is consistently enabled for Microsoft Defender for Cloud across all your Azure subscriptions.
