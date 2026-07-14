# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This project demonstrates how Amazon S3 storage can be managed using both AWS CLI and Python boto3.

The task involved setting up AWS tools on an Ubuntu EC2 instance and automating S3 operations using Python scripts.

The main objectives were:

- Configure AWS CLI and AWS authentication
- Create and manage S3 buckets
- Upload and download files from S3
- Delete S3 objects and buckets
- Automate S3 management using Python boto3

---

# 🛠️ Environment Setup

The task was completed using:

- AWS EC2 Ubuntu 24.04 LTS instance
- AWS CLI
- Python 3
- Python virtual environment
- boto3 AWS SDK

AWS CLI was installed and configured using:

```bash
aws configure

This allowed the EC2 instance to authenticate and communicate with AWS services.

📸 Screenshot:
AWS CLI setup and authentication

🪣 AWS CLI S3 Management

AWS CLI was used to manually interact with S3 storage.

Completed operations:

Created an S3 bucket
Listed available buckets
Uploaded files to S3
Checked bucket contents
Downloaded files from S3
Removed S3 objects
Removed S3 buckets

Example commands used:

aws s3 mb s3://bucket-name

Creates an S3 bucket.

aws s3 cp file.txt s3://bucket-name

Uploads a file to S3.

aws s3 ls s3://bucket-name

Lists objects stored in a bucket.

📸 Screenshots:

S3 bucket creation
File upload
Bucket contents
🐍 Python boto3 Automation

After configuring AWS CLI, boto3 was installed inside a Python virtual environment.

boto3 was used to automate S3 management tasks.

The following scripts were created:

Script	Purpose
list_buckets.py	Lists all S3 buckets
create_bucket.py	Creates an S3 bucket
upload_file.py	Uploads a file to S3
download_file.py	Downloads a file from S3
delete_file.py	Deletes an S3 object
delete_bucket.py	Deletes an S3 bucket
🚀 Completed boto3 Operations
List S3 Buckets

Used boto3 to retrieve available S3 buckets.

📸 Screenshot:
boto3 bucket listing

Create S3 Bucket

Created:

tech610-suhaib-test-boto3

📸 Screenshot:
boto3 bucket creation

Upload File

Uploaded:

test.txt

Output:

Uploaded test.txt to tech610-suhaib-test-boto3

📸 Screenshot:
boto3 upload successful

Download File

Retrieved the file from S3 back to the EC2 instance.

Output:

Downloaded test.txt from tech610-suhaib-test-boto3

📸 Screenshot:
boto3 download successful

Delete S3 Object

Removed the uploaded file from the bucket.

📸 Screenshot:
boto3 object deletion

Delete S3 Bucket

Deleted the S3 bucket after removing its contents.

📸 Screenshot:
boto3 bucket deletion

📁 Project Structure
s3-boto3-task/

├── README.md
├── list_buckets.py
├── create_bucket.py
├── upload_file.py
├── download_file.py
├── delete_file.py
└── delete_bucket.py

📸 Screenshot:
Project folder showing scripts

✅ Final Outcome

Successfully completed AWS S3 management using:

AWS CLI for manual S3 operations
Python boto3 for automation

The project demonstrates the ability to:

Configure AWS services
Manage cloud storage resources
Automate AWS tasks using Python
Work with AWS SDKs and APIs
