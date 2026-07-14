# ☁️ AWS S3 Storage Management Using AWS CLI and Python boto3

## 📌 Task Overview

This project demonstrates how Amazon S3 storage was managed using both AWS CLI and Python boto3 on an Ubuntu 24.04 LTS EC2 instance.

The task involved configuring AWS tools, authenticating with AWS, manually managing S3 resources using AWS CLI, and automating the same operations using Python scripts.

The main objectives were:

- Configure AWS CLI and AWS authentication
- Create and manage S3 buckets
- Upload and download files from S3
- Delete S3 objects and buckets
- Automate S3 management using Python boto3

---

# 🎯 Learning Outcomes

By completing this task, I gained practical experience with:

- Installing and configuring AWS CLI
- Authenticating AWS services using `aws configure`
- Managing S3 buckets and objects using AWS CLI
- Creating Python virtual environments
- Installing and using Python boto3
- Automating AWS S3 operations using Python scripts

---

# 🛠️ Environment Setup

The project was completed using:

- Ubuntu 24.04 LTS EC2 instance
- AWS CLI
- Python 3
- Python Virtual Environment (`venv`)
- Python boto3

AWS CLI was configured using:

```bash
aws configure
```

This allowed the EC2 instance to authenticate and communicate with AWS services.

A Python virtual environment was created to install boto3 safely:

```bash
python3 -m venv venv

source venv/bin/activate

pip install boto3
```

---

# 🪣 AWS CLI Commands to Manipulate S3 Storage

AWS CLI was used to manually manage S3 storage by creating buckets, uploading files, downloading files, and deleting resources.

---

## List S3 Buckets

View available S3 buckets:

```bash
aws s3 ls
```

---

## AWS CLI Help Commands

View available S3 commands:

```bash
aws s3 help
```

View help for a specific command:

```bash
aws s3 mb help
```

---

## Create an S3 Bucket

Create a new bucket:

```bash
aws s3 mb s3://tech610-suhaib-first-bucket
```

---

## List Files Inside a Bucket

View objects stored inside a bucket:

```bash
aws s3 ls s3://tech610-suhaib-first-bucket
```

---

## Upload a File to S3

Create a test file:

```bash
echo "This is the first line in a test file" > test.txt
```

View file contents:

```bash
cat test.txt
```

Upload the file:

```bash
aws s3 cp test.txt s3://tech610-suhaib-first-bucket
```

---

## Download Files from S3

Create a download folder:

```bash
mkdir downloads
cd downloads
```

Download files from S3:

```bash
aws s3 sync s3://tech610-suhaib-first-bucket .
```

---

## Delete S3 Objects

Delete a single file:

```bash
aws s3 rm s3://tech610-suhaib-first-bucket/test.txt
```

Delete all objects inside a bucket:

```bash
aws s3 rm s3://tech610-suhaib-first-bucket --recursive
```

This removes all objects stored inside the bucket.

---

## Delete an S3 Bucket

Delete an empty bucket:

```bash
aws s3 rb s3://tech610-suhaib-first-bucket
```

Delete a bucket and all contents:

```bash
aws s3 rb s3://tech610-suhaib-first-bucket --force
```

This removes the bucket and all objects stored inside it.

---

# 🐍 Python boto3 Automation

After configuring AWS CLI, Python boto3 was used to automate S3 management through separate Python scripts.

Each script was created to complete one specific S3 operation.

| Script | Purpose |
|---|---|
| `list_buckets.py` | Lists all S3 buckets |
| `create_bucket.py` | Creates an S3 bucket |
| `upload_file.py` | Uploads a file to S3 |
| `download_file.py` | Downloads a file from S3 |
| `delete_file.py` | Deletes an S3 object |
| `delete_bucket.py` | Deletes an S3 bucket |

---

# 🚀 Completed boto3 Tasks

The following S3 operations were completed successfully using Python boto3:

---

## List and Create S3 Bucket

Used boto3 to view available buckets and create a new bucket:

```
tech610-suhaib-test-boto3
```

---

## Upload File Using boto3

The `upload_file.py` script was used to upload:

```
test.txt
```

Example output:

```
Uploaded test.txt to tech610-suhaib-test-boto3
```

---

## Download File Using boto3

The `download_file.py` script was used to retrieve the file from S3.

Example output:

```
Downloaded test.txt from tech610-suhaib-test-boto3
```

---

## Delete S3 Object Using boto3

The `delete_file.py` script was used to remove the uploaded object from the S3 bucket.

---

## Delete S3 Bucket Using boto3

The `delete_bucket.py` script was used to remove the S3 bucket after the object was deleted.

---

# 📁 Project Structure

The completed project contains the following files:

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

The following Python boto3 scripts were created and used during this task:

- `list_buckets.py` – Lists available S3 buckets
- `create_bucket.py` – Creates an S3 bucket
- `upload_file.py` – Uploads a file to S3
- `download_file.py` – Downloads a file from S3
- `delete_file.py` – Deletes an S3 object
- `delete_bucket.py` – Deletes an S3 bucket

---

# ✅ Final Outcome

This project successfully demonstrates how to manage Amazon S3 storage using:

- AWS CLI for manual S3 operations
- Python boto3 for automation

The completed solution includes:

- AWS authentication setup
- S3 bucket creation and management
- File upload and download operations
- Object and bucket deletion
- Python automation using separate boto3 scripts

This demonstrates the ability to manage cloud storage resources and automate common S3 tasks using Python.
