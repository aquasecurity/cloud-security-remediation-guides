[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# CloudSploit Security Remediation Guides

CloudSploit's remediation guides are intended to be an open-source resource for improving cloud security. Many cloud IaaS providers like AWS, Azure, and Google Cloud have a shared responsibility model. They provide the physical and architectural security, along with tools to properly secure the services they offer, but it is up to the user to configure those settings properly.

## Background

This repository is an extension of CloudSploit's [open-source scanning engine](https://github.com/cloudsploit/scans). We first released the scanning engine in 2015, and this documentation repository is a natural follow up to that tool. The goal of these guides are to provide detailed steps on remediation common security issues in cloud services.

## Table of Contents

* AWS
    * ACM
        * [ACM Certificate Validation](en/aws/acm/acm-certificate-validation.md)
    * AutoScaling
        * [ASG Multiple AZ](en/aws/autoscaling/asg-multiple-az.md)
    * CloudFront
        * [CloudFront HTTPS Only](en/aws/cloudfront/cloudfront-https-only.md)
        * [CloudFront Logging Enabled](en/aws/cloudfront/cloudfront-logging-enabled.md)
        * [Insecure CloudFront Protocols](en/aws/cloudfront/insecure-cloudfront-protocols.md)
        * [Public S3 CloudFront Origin](en/aws/cloudfront/public-s3-cloudfront-origin.md)
        * [Secure CloudFront Origin](en/aws/cloudfront/secure-cloudfront-origin.md)
    * CloudTrail
        * [CloudTrail Bucket Access Logging](en/aws/cloudtrail/cloudtrail-bucket-access-logging.md)
        * [CloudTrail Bucket Delete Policy](en/aws/cloudtrail/cloudtrail-bucket-delete-policy.md)
        * [CloudTrail Bucket Private](en/aws/cloudtrail/cloudtrail-bucket-private.md)
        * [CloudTrail Enabled](en/aws/cloudtrail/cloudtrail-enabled.md)
        * [CloudTrail Encryption](en/aws/cloudtrail/cloudtrail-encryption.md)
        * [CloudTrail File Validation](en/aws/cloudtrail/cloudtrail-file-validation.md)
        * [CloudTrail To CloudWatch](en/aws/cloudtrail/cloudtrail-to-cloudwatch.md)
    * CloudWatchLogs
        * [CloudWatch Monitoring Metrics](en/aws/cloudwatchlogs/cloudwatch-monitoring-metrics.md)
    * ConfigService
        * [Config Service Enabled](en/aws/configservice/config-service-enabled.md)
    * EC2
        * [Cross VPC Public Private Communication](en/aws/ec2/cross-vpc-public-private-communication.md)
        * [Default Security Group](en/aws/ec2/default-security-group.md)
        * [Default VPC In Use](en/aws/ec2/default-vpc-in-use.md)
        * [Detect EC2 Classic Instances](en/aws/ec2/detect-ec2-classic-instances.md)
        * [EBS Encrypted Snapshots](en/aws/ec2/ebs-encrypted-snapshots.md)
        * [EBS Encryption Enabled](en/aws/ec2/ebs-encryption-enabled.md)
        * [EC2 Instance Key Based Login](en/aws/ec2/ec2-instance-key-based-login.md)
        * [EC2 Max Instances](en/aws/ec2/ec2-max-instances.md)
        * [Elastic IP Limit](en/aws/ec2/elastic-ip-limit.md)
        * [Encrypted AMI](en/aws/ec2/encrypted-ami.md)
        * [Excessive Security Groups](en/aws/ec2/excessive-security-groups.md)
        * [Instance IAM Role](en/aws/ec2/instance-iam-role.md)
        * [Instance Limit](en/aws/ec2/instance-limit.md)
        * [NAT Multiple AZ](en/aws/ec2/nat-multiple-az.md)
        * [Open All Ports Protocols](en/aws/ec2/open-all-ports-protocols.md)
        * [Open CIFS](en/aws/ec2/open-cifs.md)
        * [Open DNS](en/aws/ec2/open-dns.md)
        * [Open Elasticsearch](en/aws/ec2/open-elasticsearch.md)
        * [Open FTP](en/aws/ec2/open-ftp.md)
        * [Open MySQL](en/aws/ec2/open-mysql.md)
        * [Open NetBIOS](en/aws/ec2/open-netbios.md)
        * [Open Oracle](en/aws/ec2/open-oracle.md)
        * [Open PostgreSQL](en/aws/ec2/open-postgresql.md)
        * [Open RDP](en/aws/ec2/open-rdp.md)
        * [Open RPC](en/aws/ec2/open-rpc.md)
        * [Open SMBoTCP](en/aws/ec2/open-smbotcp.md)
        * [Open SMTP](en/aws/ec2/open-smtp.md)
        * [Open SQL Server](en/aws/ec2/open-sql-server.md)
        * [Open SSH](en/aws/ec2/open-ssh.md)
        * [Open Telnet](en/aws/ec2/open-telnet.md)
        * [Open VNC Client](en/aws/ec2/open-vnc-client.md)
        * [Open VNC Server](en/aws/ec2/open-vnc-server.md)
        * [Overlapping Security Groups](en/aws/ec2/overlapping-security-groups.md)
        * [Public AMI](en/aws/ec2/public-ami.md)
        * [Subnet IP Availability](en/aws/ec2/subnet-ip-availability.md)
        * [VPC Elastic IP Limit](en/aws/ec2/vpc-elastic-ip-limit.md)
        * [VPC Flow Logs Enabled](en/aws/ec2/vpc-flow-logs-enabled.md)
        * [VPC Multiple Subnets](en/aws/ec2/vpc-multiple-subnets.md)
    * ELB
        * [ELB HTTPS Only](en/aws/elb/elb-https-only.md)
        * [ELB Logging Enabled](en/aws/elb/elb-logging-enabled.md)
        * [ELB No Instances](en/aws/elb/elb-no-instances.md)
        * [Insecure Ciphers](en/aws/elb/insecure-ciphers.md)
    * Firehose
        * [Firehose Delivery Streams Encrypted](en/aws/firehose/firehose-delivery-streams-encrypted.md)
    * IAM
        * [Access Keys Extra](en/aws/iam/access-keys-extra.md)
        * [Access Keys Last Used](en/aws/iam/access-keys-last-used.md)
        * [Access Keys Rotated](en/aws/iam/access-keys-rotated.md)
        * [Certificate Expiry](en/aws/iam/certificate-expiry.md)
        * [Empty Groups](en/aws/iam/empty-groups.md)
        * [IAM User Admins](en/aws/iam/iam-user-admins.md)
        * [Maximum Password Age](en/aws/iam/maximum-password-age.md)
        * [Minimum Password Length](en/aws/iam/minimum-password-length.md)
        * [No User IAM Policies](en/aws/iam/no-user-iam-policies.md)
        * [Password Expiration](en/aws/iam/password-expiration.md)
        * [Password Requires Lowercase](en/aws/iam/password-requires-lowercase.md)
        * [Password Requires Numbers](en/aws/iam/password-requires-numbers.md)
        * [Password Requires Symbols](en/aws/iam/password-requires-symbols.md)
        * [Password Requires Uppercase](en/aws/iam/password-requires-uppercase.md)
        * [Password Reuse Prevention](en/aws/iam/password-reuse-prevention.md)
        * [Root Access Keys](en/aws/iam/root-access-keys.md)
        * [Root Account In Use](en/aws/iam/root-account-in-use.md)
        * [Root MFA Enabled](en/aws/iam/root-mfa-enabled.md)
        * [SSH Keys Rotated](en/aws/iam/ssh-keys-rotated.md)
        * [Users MFA Enabled](en/aws/iam/users-mfa-enabled.md)
        * [Users Password Last Used](en/aws/iam/users-password-last-used.md)
    * KMS
        * [KMS Default Key Usage](en/aws/kms/kms-default-key-usage.md)
        * [KMS Key Policy](en/aws/kms/kms-key-policy.md)
        * [KMS Key Rotation](en/aws/kms/kms-key-rotation.md)
        * [KMS Scheduled Deletion](en/aws/kms/kms-scheduled-deletion.md)
    * Kinesis
        * [Kinesis Streams Encrypted](en/aws/kinesis/kinesis-streams-encrypted.md)
    * Lambda
        * [Lambda Old Runtimes](en/aws/lambda/lambda-old-runtimes.md)
    * RDS
        * [RDS Automated Backups](en/aws/rds/rds-automated-backups.md)
        * [RDS Encryption Enabled](en/aws/rds/rds-encryption-enabled.md)
        * [RDS Multiple AZ](en/aws/rds/rds-multiple-az.md)
        * [RDS Publicly Accessible](en/aws/rds/rds-publicly-accessible.md)
        * [RDS Restorable](en/aws/rds/rds-restorable.md)
    * Redshift
        * [Redshift Encryption Enabled](en/aws/redshift/redshift-encryption-enabled.md)
        * [Redshift Publicly Accessible](en/aws/redshift/redshift-publicly-accessible.md)
    * Route53
        * [Domain Auto Renew](en/aws/route53/domain-auto-renew.md)
        * [Domain Expiry](en/aws/route53/domain-expiry.md)
        * [Domain Transfer Lock](en/aws/route53/domain-transfer-lock.md)
    * S3
        * [S3 Bucket All Users ACL](en/aws/s3/s3-bucket-all-users-acl.md)
        * [S3 Bucket All Users Policy](en/aws/s3/s3-bucket-all-users-policy.md)
        * [S3 Bucket Logging](en/aws/s3/s3-bucket-logging.md)
        * [S3 Bucket Versioning](en/aws/s3/s3-bucket-versioning.md)
    * SES
        * [Email DKIM Enabled](en/aws/ses/email-dkim-enabled.md)
    * SNS
        * [SNS Topic Policies](en/aws/sns/sns-topic-policies.md)
    * SQS
        * [SQS Cross Account Access](en/aws/sqs/sqs-cross-account-access.md)
        * [SQS Encrypted](en/aws/sqs/sqs-encrypted.md)
    * SSM
        * [SSM Encrypted Parameters](en/aws/ssm/ssm-encrypted-parameters.md)
    * SageMaker
        * [Notebook Data Encrypted](en/aws/sagemaker/notebook-data-encrypted.md)
        * [Notebook Direct Internet Access](en/aws/sagemaker/notebook-direct-internet-access.md)
* Azure
    * App Service
        * [.NET Framework Version](en/azure/appservice/.net-framework-version.md)
        * [Authentication Enabled](en/azure/appservice/authentication-enabled.md)
        * [Client Certificates Enabled](en/azure/appservice/client-certificates-enabled.md)
        * [HTTP 2.0 Enabled](en/azure/appservice/http-2.0-enabled.md)
        * [HTTPS Only Enabled](en/azure/appservice/https-only-enabled.md)
        * [Identity Enabled](en/azure/appservice/identity-enabled.md)
        * [Python Version](en/azure/appservice/python-version.md)
    * Azure Policy
        * [Resource Location Matches Resource Group](en/azure/azurepolicy/resource-location-matches-resource-group.md)
        * [Resources Allowed Locations](en/azure/azurepolicy/resources-allowed-locations.md)
    * Blob Service
        * [Blob Container Private Access](en/azure/blobservice/blob-container-private-access.md)
        * [Blob Service Immutable](en/azure/blobservice/blob-service-immutable.md)
    * CDN
        * [Detect Insecure Custom Origin](en/azure/cdn/detect-insecure-custom-origin.md)
    * File Service
        * [File Service All Access ACL](en/azure/fileservice/file-service-all-access-acl.md)
    * Key Vault
        * [Key Expiration Enabled](en/azure/keyvault/key-expiration-enabled.md)
    * Kubernetes Service
        * [RBAC Enabled](en/azure/kubernetesservice/rbac-enabled.md)
    * Log Alerts
        * [SQL Server Firewall Rule Alerts Monitor](en/azure/logalerts/sql-server-firewall-rule-alerts-monitor.md)
        * [Virtual Network Alerts Monitor](en/azure/logalerts/virtual-network-alerts-monitor.md)
    * Monitor
        * [Autoscale Enabled](en/azure/monitor/autoscale-enabled.md)
        * [Log Profile Archive Data](en/azure/monitor/log-profile-archive-data.md)
        * [NSG Log Analytics Enabled](en/azure/monitor/nsg-log-analytics-enabled.md)
    * MySQL Server
        * [Enforce SSL Connection Enabled](en/azure/mysqlserver/enforce-ssl-connection-enabled.md)
    * Network Security Groups
        * [Default Security Group](en/azure/networksecuritygroups/default-security-group.md)
        * [Open All Ports](en/azure/networksecuritygroups/open-all-ports.md)
        * [Open CIFS](en/azure/networksecuritygroups/open-cifs.md)
        * [Open DNS](en/azure/networksecuritygroups/open-dns.md)
        * [Open FTP](en/azure/networksecuritygroups/open-ftp.md)
        * [Open Hadoop HDFS NameNode Metadata Service](en/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service.md)
        * [Open Hadoop HDFS NameNode WebUI](en/azure/networksecuritygroups/open-hadoop-hdfs-namenode-webui.md)
        * [Open Kibana](en/azure/networksecuritygroups/open-kibana.md)
        * [Open MySQL](en/azure/networksecuritygroups/open-mysql.md)
        * [Open NetBIOS](en/azure/networksecuritygroups/open-netbios.md)
        * [Open Oracle](en/azure/networksecuritygroups/open-oracle.md)
        * [Open PostgreSQL](en/azure/networksecuritygroups/open-postgresql.md)
        * [Open RDP](en/azure/networksecuritygroups/open-rdp.md)
        * [Open RPC](en/azure/networksecuritygroups/open-rpc.md)
        * [Open SMBoTCP](en/azure/networksecuritygroups/open-smbotcp.md)
        * [Open SMTP](en/azure/networksecuritygroups/open-smtp.md)
        * [Open SQLServer](en/azure/networksecuritygroups/open-sqlserver.md)
        * [Open SSH](en/azure/networksecuritygroups/open-ssh.md)
        * [Open Telnet](en/azure/networksecuritygroups/open-telnet.md)
        * [Open VNC Client](en/azure/networksecuritygroups/open-vnc-client.md)
        * [Open VNC Server](en/azure/networksecuritygroups/open-vnc-server.md)
    * Queue Service
        * [Queue Service All Access ACL](en/azure/queueservice/queue-service-all-access-acl.md)
    * SQL Server
        * [TDE Protector Encrypted](en/azure/sqlserver/tde-protector-encrypted.md)
    * Security Center
        * [Application Whitelisting Enabled](en/azure/securitycenter/application-whitelisting-enabled.md)
        * [Monitor Blob Encryption](en/azure/securitycenter/monitor-blob-encryption.md)
        * [Monitor Disk Encryption](en/azure/securitycenter/monitor-disk-encryption.md)
        * [Monitor SQL Auditing](en/azure/securitycenter/monitor-sql-auditing.md)
        * [Monitor SQL Encryption](en/azure/securitycenter/monitor-sql-encryption.md)
        * [Monitor VM Vulnerability](en/azure/securitycenter/monitor-vm-vulnerability.md)
        * [Security Configuration Monitoring](en/azure/securitycenter/security-configuration-monitoring.md)
    * Storage Accounts
        * [Log Container Public Access](en/azure/storageaccounts/log-container-public-access.md)
        * [Log Storage Encryption](en/azure/storageaccounts/log-storage-encryption.md)
        * [Network Access Default Action](en/azure/storageaccounts/network-access-default-action.md)
        * [Storage Accounts Encryption](en/azure/storageaccounts/storage-accounts-encryption.md)
        * [Storage Accounts HTTPS](en/azure/storageaccounts/storage-accounts-https.md)
    * Table Service
        * [Table Service All Access ACL](en/azure/tableservice/table-service-all-access-acl.md)
    * Virtual Machines
        * [VM Agent Enabled](en/azure/virtualmachines/vm-agent-enabled.md)
        * [VM Auto Update Enabled](en/azure/virtualmachines/vm-auto-update-enabled.md)
        * [VM Data Disk Encryption](en/azure/virtualmachines/vm-data-disk-encryption.md)
        * [VM Endpoint Protection](en/azure/virtualmachines/vm-endpoint-protection.md)
        * [VM OS Disk Encryption](en/azure/virtualmachines/vm-os-disk-encryption.md)

## Contributing

Please see the [contributor's guide](.github/CONTRIBUTING.md).