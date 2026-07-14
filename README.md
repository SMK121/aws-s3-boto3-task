# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This task demonstrates how to set up and manage Amazon S3 storage using both the AWS Command Line Interface (CLI) and Python boto3.

The aim was to:

- Configure AWS CLI on an Ubuntu EC2 instance
- Authenticate AWS services using AWS credentials
- Create and manage S3 resources using AWS CLI
- Automate S3 operations using Python boto3
- Perform the full S3 lifecycle:
  - Create a bucket
  - Upload files
  - Download files
  - Delete objects
  - Delete buckets

---

# 🎯 Objectives / Outcomes

By completing this task, I was able to:

- Install and configure AWS CLI
- Authenticate AWS access using `aws configure`
- Manage S3 storage using AWS CLI commands
- Set up a Python virtual environment
- Install and use the boto3 AWS SDK
- Create Python scripts to automate S3 operations
- Upload, retrieve, and remove S3 objects programmatically

---

# 🛠️ AWS CLI Setup

## Install AWS CLI

AWS CLI was installed on the Ubuntu EC2 instance to allow command-line interaction with AWS services.

Commands used:

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

unzip awscliv2.zip

sudo ./aws/install
