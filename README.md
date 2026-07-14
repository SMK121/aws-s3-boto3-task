# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This task demonstrates how to set up and manage Amazon S3 storage using both the AWS Command Line Interface (CLI) and Python boto3.

The aim was to:

- 🖥️ Configure AWS tools on an Ubuntu EC2 instance
- 🔐 Authenticate AWS CLI access
- 🪣 Create and manage S3 resources using AWS CLI commands
- 🐍 Use Python boto3 to automate S3 bucket and object management
- 🔄 Perform the full S3 lifecycle: create, upload, download, delete files, and remove buckets

---

# 🎯 Objectives / Outcomes

By completing this task, I was able to:

- ⚙️ Install and configure AWS CLI on an Ubuntu EC2 instance
- 🔑 Authenticate AWS services using AWS credentials
- 🪣 Create and manipulate S3 buckets using AWS CLI
- 🐍 Set up a Python environment for AWS automation
- 📦 Install and use the boto3 AWS SDK for Python
- 📝 Create Python scripts to manage S3 resources
- ⬆️ Upload and retrieve files from S3 using Python
- 🗑️ Delete S3 objects and buckets programmatically

---

# 🖥️ Environment Setup

## ☁️ EC2 Instance

The work was completed on an Ubuntu 24.04 LTS EC2 instance.

Instance details:

- 🐧 Operating System: Ubuntu 24.04 LTS
- 💻 Instance Type: t3.micro
- 🌍 AWS Region: eu-west-1
 
---

# 🛠️ AWS CLI Setup

## 📥 Install AWS CLI

AWS CLI was installed on the EC2 instance to allow interaction with AWS services from the command line.

Commands used:

```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

unzip awscliv2.zip

sudo ./aws/install
