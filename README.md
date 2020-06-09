# Relay Workflows  
This repository contains workflows for [Relay](https://relay.sh). Feel free to use these workflows to get started.

| Category | Workflow      | Integrations  | Description  | Try it! |
| ------------- | ------------- | ------------- | ------------ | -- |
| Cost Optimization | [Terminate EC2 instances without valid lifetime tag](./ec2-reaper) | aws-ec2 | Terminates EC2 instances not in compliance with a tagging policy: specifying a `lifetime` or `termination_date` tag. | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=ec2-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fec2-reaper%2Fec2-reaper.yaml) |
| Cost Optimization | [Delete unattached EBS volumes](./ebs-reaper) | aws-ebs | Deletes EBS volumes that are unattached | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=ebs-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Febs-reaper%2Febs-reaper.yaml) |
| Cost Optimization | [Delete empty ELBv2 load balancers](./elbv2-delete-empty-loadbalancers) | aws-elbv2 | Deletes empty ELBv2 load balancers | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=delete-empty-elbv2-loadbalancers&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Felbv2-delete-empty-loadbalancers%2Felbv2-delete-empty-loadbalancers.yaml) |
| Cost Optimization | [Delete unattached Azure Disks](./azure-disk-reaper) | azure-disks | Deletes Azure Disks that are unattached | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=azure-disk-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-disk-reaper%2Fazure-disk-reaper.yaml) |  
| Cost Optimization | [Delete untagged Azure Virtual Machines](./azure-vm-reaper) | azure-virtual-machines | Deletes Azure Virtual Machines that don't have any tags | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=azure-vm-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-vm-reaper%2Fazure-vm-reaper.yaml) |
| Cost Optimization | [Delete empty Azure Load Balancers](./azure-delete-empty-loadbalancers) | azure-network | Deletes empty Azure Load Balancers | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=azure-delete-empty-lbs&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-delete-empty-loadbalancers%2Fazure-delete-empty-loadbalancers.yaml) |
| Cost Optimization | [Delete unused Azure Network Interfaces](./azure-delete-unused-nics) | azure-network | Deletes unused Azure Network Interfaces | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=azure-delete-unused-nics&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-delete-unused-nics%2Fazure-delete-unused-nics.yaml) |
| Cost Optimization | [Delete GCP instances without valid lifetime tag](./gcp-instance-reaper) | gcp-instances | Deletes GCP instances not in compliance with a tagging policy: specifying a `lifetime` or `termination_date` tag. | |
| Incident Response | [When a Datadog event is received, send a message to Slack](./datadog-to-slack) | datadog, slack | Sends a message to Slack when a Datadog event is received| [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=datadog-to-slack&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fdatadog-to-slack%2Fdatadog-to-slack.yaml) |
| Incident Response | [When a Datadog event is received, create a Jira issue](./datadog-to-jira) | datadog, jira-server | Creates a Jira Server issue when a Datadog event is received | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=datadog-to-jira&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fdatadog-to-jira%2Fdatadog-to-jira.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, send a message to Slack](./pagerduty-to-slack) | pagerduty, slack | Sends a message to Slack when a PagerDuty incident is triggered based on incident severity| [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=pagerduty-to-slack&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-slack%2Fpagerduty-to-slack.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, create a Jira ticket](./pagerduty-to-jira) | pagerduty, jira-server | Creates a Jira Server issue when a PagerDuty incident is triggered | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=pagerduty-to-jira&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-jira%2Fpagerduty-to-jira.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, send an SMS via Twilio](./pagerduty-to-twilio) | pagerduty, twilio | Deliver a custom notification via SMS when a PagerDuty incident is triggered | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://nebula.puppet.com/create-workflow?workflowName=pagerduty-to-twilio&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-twilio%2Fpagerduty-to-twilio.yaml) |
| Security | [Stop untagged EC2 instances](./ec2-stop-untagged-instances) | aws-ec2 | Stops untagged EC2 instances | 
| Security | [Restrict public WRITE S3 buckets](./s3-restrict-public-write-buckets) | aws-s3 | Finds all buckets with public 'WRITE' permissions and marks them `private` | 
| Security | [Restrict public READ S3 buckets](./s3-restrict-public-read-buckets) | aws-s3 | Finds all buckets with public 'READ' permissions and marks them `private` | 
| Security | [Restrict public WRITE_ACP S3 buckets](./s3-restrict-public-write_acp-buckets) | aws-s3 | Finds all buckets with public 'WRITE_ACP' permissions and marks them `private` | 
| Security | [Restrict public READ_ACP S3 buckets](./s3-restrict-public-read_acp-buckets) | aws-s3 | Finds all buckets with public 'READ_ACP' permissions and marks them `private` | 
| Security | [Restrict S3 buckets with READ access to all Authenticated Users](./s3-restrict-authenticated_user-read-buckets) | aws-s3 | Finds all buckets with 'READ' permissions to all Authenticated Users and marks them `private` | 
| Security | [Restrict S3 buckets with WRITE access to all Authenticated Users](./s3-restrict-authenticated_user-write-buckets) | aws-s3 | Finds all buckets with 'WRITE' permissions to all Authenticated Users and marks them `private` | 
| Security | [Restrict S3 buckets with READ_ACP access to all Authenticated Users](./s3-restrict-authenticated_user-read_acp-buckets) | aws-s3 | Finds all buckets with 'READ_ACP' permissions to all Authenticated Users and marks them `private` | 
| Security | [Restrict S3 buckets with WRITE_ACP access to all Authenticated Users](./s3-restrict-authenticated_user-write_acp-buckets) | aws-s3 | Finds all buckets with 'WRITE_ACP' permissions to all Authenticated Users and marks them `private` | 
| Security | [Remediate unencrypted S3 buckets](./s3-remediate-unencrypted-buckets) | aws-s3 | Finds all unencrypted S3 buckets and encrypts them with default encryption | 
| Security | [Remove unused EC2 key pairs](./ec2-remove-unused-key-pairs) | aws-ec2 | Finds all unused EC2 key pairs and deletes them | 
| Continuous Delivery | [Run Terraform when Pull Request merged in GitHub](./terraform-continuous-deployment) | terraform, github | Run Terraform command {plan, apply, etc} when a Pull Request is merged to a repository in GitHub. | |
| Continuous Delivery | [Update Kubernetes deployment image tag on Docker Hub push](./kubectl-apply-on-dockerhub-push) | Kubernetes | Updates a deployment image using a Docker Hub webhook to inform relay when a new Docker image is available |
| Provisioning | [Provision an EC2 instance and configure with a Bolt plan](./ec2-provision-and-configure-with-bolt) | aws-ec2 | Uses terraform to create and provision a new EC2 instance, then uses a remote Bolt plan to configure it |
