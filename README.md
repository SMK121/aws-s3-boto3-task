# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This project demonstrates how Amazon S3 storage can be managed using both AWS CLI and the Python boto3 on an Ubuntu 24.04 LTS EC2 instance.

The task included configuring AWS CLI, authenticating with AWS, managing S3 resources manually, and automating the same operations using Python scripts.

---

# 🎯 Learning Outcomes

By completing this task, I was able to:

- Install and configure AWS CLI
- Authenticate AWS services using `aws configure`
- Manage S3 buckets and objects using AWS CLI
- Set up a Python virtual environment
- Install and use the boto3 AWS SDK
- Automate S3 operations using Python

---

# 🛠️ Environment Setup

The project was completed using:

- Ubuntu 24.04 LTS EC2 instance
- AWS CLI
- Python 3
- Python Virtual Environment (`venv`)
- boto3

AWS CLI was configured using:

```bash
aws configure
```

A Python virtual environment was created and boto3 installed:

```bash
python3 -m venv venv

source venv/bin/activate

pip install boto3
```

---

# 🪣 AWS CLI S3 Management

AWS CLI was used to perform manual S3 operations including:

- Creating an S3 bucket
- Listing S3 buckets
- Uploading files
- Viewing bucket contents
- Downloading files
- Deleting S3 objects
- Deleting S3 buckets

Example commands:

```bash
aws s3 mb s3://bucket-name

aws s3 ls

aws s3 cp test.txt s3://bucket-name

aws s3 cp s3://bucket-name/test.txt .

aws s3 rm s3://bucket-name/test.txt

aws s3 rb s3://bucket-name
```

---

# 🐍 Python boto3 Automation

After configuring AWS CLI, boto3 was used to automate S3 management through simple Python scripts.

Each script performs one task without unnecessary complexity.

| Script | Purpose |
|---------|---------|
| `list_buckets.py` | List all S3 buckets |
| `create_bucket.py` | Create an S3 bucket |
| `upload_file.py` | Upload a file to S3 |
| `download_file.py` | Download a file from S3 |
| `delete_file.py` | Delete an object from S3 |
| `delete_bucket.py` | Delete an S3 bucket |

---

# 🚀 Completed boto3 Tasks

The following operations were completed successfully using Python boto3:

- Listed available S3 buckets
- Created a new S3 bucket
- Uploaded `test.txt`
- Downloaded `test.txt`
- Deleted the uploaded object
- Deleted the S3 bucket

---

# 📁 Project Structure

```
s3-boto3-task/

├── README.md
├── list_buckets.py
├── create_bucket.py
├── upload_file.py
├── download_file.py
├── delete_file.py
├── delete_bucket.py
└── test.txt
```

---

# 🔗 Python Scripts Used

The following Python boto3 scripts were created and used to automate S3 management tasks:

- `list_buckets.py` – Lists all S3 buckets.
- `create_bucket.py` – Creates an S3 bucket.
- `upload_file.py` – Uploads a file to an S3 bucket.
- `download_file.py` – Downloads a file from an S3 bucket.
- `delete_file.py` – Deletes an object from an S3 bucket.
- `delete_bucket.py` – Deletes an S3 bucket.

---

# ✅ Final Outcome

This project successfully demonstrates how to manage Amazon S3 storage using both AWS CLI and Python boto3.

The completed solution includes:

- AWS CLI installation and authentication
- S3 bucket creation and management
- File upload and download
- Object and bucket deletion
- Python automation using six separate boto3 scripts

This project provides a simple example of using the AWS SDK for Python to automate common cloud storage tasks.
