# Contributing to CloudSploit Remediation Guides

Thank you for your contributions to the CloudSploit Remediation Guide. This repository exists as an open source knowledge base of cloud (AWS and Azure) security guidelines to remediate common misconfigurations.

## Repo Format

This repository uses the following layout:
```
|_remediations
	|_langugage (e.g. en)
		|_cloud (e.g. aws)
			|_category (e.g acm)
				|_guide.md
```

## Guidelines for New Pages

Please ensure that your contributions include the following:

1. Each new guide should begin with the CloudSploit logo code:
```
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)
```
2. The title should follow the following format:
```
# Cloud / Category / Remediation Guide
```
For example:
```
# AWS / ACM / ACM Certificate Validation
```
3. A `## Quick Info` section containing information on the CloudSploit plugin.
4. A `## Detailed Remediation Steps` section with steps that users can follow to remediate detected issues.

## Guidelines for Adding Steps

To ensure consistent quality, please follow the below steps when contributing new remediation steps:

1. Steps should be clear and concise for users of AWS or Azure.
2. Steps should include details such as "Log into the AWS console" and "navigate to the EC2 page".
3. Describe the process to locate the detected misconfiguration or vulnerability.
4. Include as many screenshots as possible.
5. Describe how the user can verify the fix (e.g. "ensure the security group port list has changed to x").

## Submitting Changes

Please submit each new guide or each change as a separate PR by forking this repository and using your own branches.
