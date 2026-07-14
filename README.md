# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This project demonstrates how Amazon S3 storage was managed using AWS CLI and Python boto3.

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

AWS CLI was configured using:

```bash
aws configure

This allowed the EC2 instance to authenticate and communicate with AWS services.

AWS CLI authentication (aws configure)
Successful AWS connection (aws s3 ls)
🪣 AWS CLI S3 Management

AWS CLI was used to manually manage S3 storage.

Completed operations:

Created an S3 bucket
Listed available buckets
Uploaded files to S3
Checked bucket contents
Downloaded files from S3
Removed S3 objects
Removed S3 buckets

Example commands used:

Create an S3 bucket:

aws s3 mb s3://bucket-name

Upload a file:

aws s3 cp file.txt s3://bucket-name

List objects stored in a bucket:

aws s3 ls s3://bucket-name



📸 Screenshot needed:

AWS CLI bucket creation
AWS CLI upload working
File visible inside S3 bucket
🐍 Python boto3 Setup

After configuring AWS CLI, boto3 was installed inside a Python virtual environment.

boto3 was used to automate S3 management tasks using Python scripts.

The scripts created were:

Script	Purpose
list_buckets.py	Lists all S3 buckets
create_bucket.py	Creates an S3 bucket
upload_file.py	Uploads a file to S3
download_file.py	Downloads a file from S3
delete_file.py	Deletes an S3 object
delete_bucket.py	Deletes an S3 bucket

📸 Screenshot needed:

Project folder showing all Python scripts
🚀 boto3 List and Create S3 Bucket

The list_buckets.py script was used to display available S3 buckets.

The create_bucket.py script was used to create a new S3 bucket:

tech610-suhaib-test-boto3

📸 Screenshot needed:

boto3 create bucket working
boto3 list buckets output
📤 Upload File Using boto3

The upload_file.py script uploads a local file into the S3 bucket.

File uploaded:

test.txt

Example output:

Uploaded test.txt to tech610-suhaib-test-boto3

📸 Screenshot needed:

boto3 upload successful output
📥 Download File Using boto3

The download_file.py script retrieves a file from S3 back to the EC2 instance.

Example output:

Downloaded test.txt from tech610-suhaib-test-boto3

📸 Screenshot needed:

boto3 download successful output
🗑️ Delete S3 Object Using boto3

The delete_file.py script removes an object from the S3 bucket.

This completes the object deletion stage of the S3 lifecycle.

📸 Screenshot needed:

boto3 deleted S3 object output
🪣 Delete S3 Bucket Using boto3

The delete_bucket.py script removes the S3 bucket after all objects have been deleted.

📸 Screenshot needed:

boto3 bucket deletion output
📁 Project Structure

The final project contains:

s3-boto3-task/

├── README.md
├── list_buckets.py
├── create_bucket.py
├── upload_file.py
├── download_file.py
├── delete_file.py
└── delete_bucket.py

📸 Screenshot needed:

VS Code project folder showing Python scripts
🔗 Python Scripts

The completed boto3 automation scripts are included in this repository:

list_buckets.py
create_bucket.py
upload_file.py
download_file.py
delete_file.py
delete_bucket.py
✅ Final Outcome

Successfully completed AWS S3 management using:

AWS CLI for manual S3 operations
Python boto3 for automation

The project demonstrates the ability to:

Configure AWS services
Authenticate using AWS credentials
Manage cloud storage resources
Automate AWS tasks using Python
