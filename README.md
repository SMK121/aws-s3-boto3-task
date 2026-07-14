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

AWS CLI was installed and configured to allow communication with AWS services.

AWS authentication was completed using:

```bash
aws configure
```

This configured AWS credentials and allowed the EC2 instance to interact with AWS resources.

📸 **Screenshot:**
- AWS CLI authentication setup
- Successful AWS connection using `aws s3 ls`

---

# 🪣 AWS CLI S3 Management

AWS CLI was used to manually interact with Amazon S3 storage.

Completed operations:

- Created an S3 bucket
- Listed S3 buckets
- Uploaded files to S3
- Checked files stored in S3
- Downloaded files from S3
- Removed S3 objects
- Removed S3 buckets

Example AWS CLI commands used:

Create an S3 bucket:

```bash
aws s3 mb s3://bucket-name
```

Upload a file:

```bash
aws s3 cp file.txt s3://bucket-name
```

List objects inside a bucket:

```bash
aws s3 ls s3://bucket-name
```

Download a file:

```bash
aws s3 cp s3://bucket-name/file.txt .
```

Delete an object:

```bash
aws s3 rm s3://bucket-name/file.txt
```

Delete a bucket:

```bash
aws s3 rb s3://bucket-name
```

📸 **Screenshots:**

- S3 bucket creation
- File upload using AWS CLI
- File visible inside S3 bucket

---

# 🐍 Python boto3 Automation

After configuring AWS CLI, a Python virtual environment was created and boto3 was installed.

boto3 is the AWS SDK for Python and was used to automate S3 management tasks.

The following Python scripts were created:

| Script | Purpose |
|---|---|
| `list_buckets.py` | Lists all S3 buckets |
| `create_bucket.py` | Creates an S3 bucket |
| `upload_file.py` | Uploads a file to S3 |
| `download_file.py` | Downloads a file from S3 |
| `delete_file.py` | Deletes an S3 object |
| `delete_bucket.py` | Deletes an S3 bucket |

---

# 🚀 Completed boto3 Operations

## List S3 Buckets

The `list_buckets.py` script was used to retrieve available S3 buckets.

📸 **Screenshot:**
- boto3 bucket listing output

---

## Create S3 Bucket

The `create_bucket.py` script created the S3 bucket:

```text
tech610-suhaib-test-boto3
```

📸 **Screenshot:**
- boto3 bucket creation output

---

## Upload File to S3

The `upload_file.py` script uploaded:

```text
test.txt
```

Example output:

```text
Uploaded test.txt to tech610-suhaib-test-boto3
```

📸 **Screenshot:**
- boto3 upload successful

---

## Download File from S3

The `download_file.py` script retrieved the file from S3 back to the EC2 instance.

Example output:

```text
Downloaded test.txt from tech610-suhaib-test-boto3
```

📸 **Screenshot:**
- boto3 download successful

---

## Delete S3 Object

The `delete_file.py` script removed the uploaded object from the S3 bucket.

📸 **Screenshot:**
- boto3 object deletion output

---

## Delete S3 Bucket

The `delete_bucket.py` script removed the S3 bucket after the objects were deleted.

📸 **Screenshot:**
- boto3 bucket deletion output

---

# 📁 Project Structure

The final project contains the following files:

```text
s3-boto3-task/

├── README.md
├── list_buckets.py
├── create_bucket.py
├── upload_file.py
├── download_file.py
├── delete_file.py
└── delete_bucket.py
```

📸 **Screenshot:**
- Project folder showing Python scripts

---

# 🔗 Python Scripts

The completed boto3 automation scripts are included in this repository:

- `list_buckets.py`
- `create_bucket.py`
- `upload_file.py`
- `download_file.py`
- `delete_file.py`
- `delete_bucket.py`

---

# ✅ Final Outcome

Successfully completed AWS S3 management using:

- AWS CLI for manual S3 operations
- Python boto3 for automation

This project demonstrates the ability to:

- Configure AWS services
- Authenticate using AWS credentials
- Manage cloud storage resources
- Automate AWS tasks using Python
- Work with AWS SDKs and APIs
