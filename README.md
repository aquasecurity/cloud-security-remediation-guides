[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# CloudSploit Security Remediation Guides

CloudSploit's remediation guides are intended to be an open-source resource for improving cloud security. Many cloud IaaS providers like AWS, Azure, and Google Cloud have a shared responsibility model. They provide the physical and architectural security, along with tools to properly secure the services they offer, but it is up to the user to configure those settings properly.

## Background

This repository is an extension of CloudSploit's [open-source scanning engine](https://github.com/cloudsploit/scans). We first released the scanning engine in 2015, and this documentation repository is a natural follow up to that tool. The goal of these guides are to provide detailed steps on remediation common security issues in cloud services.

## Contributing

We welcome and encourage contributions from the community. To contribute, please fork this repository and create a pull request with your changes. If you are adding a new security control that CloudSploit does not yet scan for, we would also love if you submitted a pull request to our scans repository as well, but it isn't required.

Please consider the following guidelines:

* Each cloud provider (AWS, Azure, etc) has its own sub-folder.
* Within each provider, there are sub-folders for the services. For example, `ec2` and `s3` for AWS.
* Each security guide has its own file with the same format and structure. Please copy an existing one for reference.
