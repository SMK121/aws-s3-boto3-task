# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This project demonstrates how to configure and manage Amazon Simple Storage Service (S3) using:

- AWS Command Line Interface (CLI)
- Python boto3 SDK

The task was completed using an Ubuntu 24.04 LTS EC2 instance.

The objectives were to:

- Install and configure AWS CLI
- Set up a Python environment with required dependencies
- Authenticate AWS services using AWS credentials
- Create and manage S3 storage using AWS CLI
- Automate S3 operations using Python boto3
- Create, upload, download, and delete S3 resources

---

# 🎯 Learning Outcomes

By completing this task, I gained practical experience with:

- AWS S3 object storage
- AWS CLI commands
- AWS authentication using IAM credentials
- Python virtual environments
- AWS SDK for Python (boto3)
- Automating cloud resource management using Python scripts

---

# 🪣 What is Amazon S3?

Amazon Simple Storage Service (S3) is AWS's object storage service used to store and retrieve data from anywhere.

## Key Features

- Stores and retrieves any amount of data
- Highly scalable and durable cloud storage
- Built-in redundancy across Availability Zones
- Can be used to host static websites
- Accessible through:
  - AWS Management Console
  - AWS CLI
  - AWS SDKs such as Python boto3

## Common Uses

S3 is commonly used for:

- Application files
- Images and videos
- Log files
- Backups
- Static website resources

By default, S3 objects are private and require permissions to allow public access.

---

# 🛠️ AWS CLI Setup

AWS CLI was installed on the Ubuntu EC2 instance to allow command-line interaction with AWS services.

---

## Update Ubuntu Packages

```bash
sudo apt update -y
