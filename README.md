# Terraform_RemoteBackendState_Using_S3
This repository is a simple Terraform setup to configure remote backend storage using Amazon S3 for the state file and DynamoDB for state locking. Ideal for collaborative infrastructure projects using Terraform on AWS.
# 🌐 Terraform Remote Backend with AWS S3 + DynamoDB

This repo sets up a **remote backend** for storing Terraform state files securely and efficiently using **Amazon S3** and **DynamoDB**.

---

## 📌 Purpose

Managing Terraform state files locally works for small projects, but for team collaboration and safety, a remote backend is essential. This setup:

- Stores state files in an S3 bucket
- Uses a DynamoDB table to enable state locking and avoid race conditions

---

## 📂 Files

| File | Description |
|------|-------------|
| `main.tf` | Defines the resources for S3 and DynamoDB |
| `variables.tf` | Input variables to configure bucket, region, etc. |
| `outputs.tf` | Exports useful values like bucket name |
| `backend-config-example.hcl` | Sample backend configuration file for usage in other projects |

---

## 🚀 How to Use

1. **Clone this repo:**

```bash
git clone https://github.com/iamkarthikumesh/Terraform_RemoteBackendState_Using_S3.git
cd Terraform_RemoteBackendState_Using_S3
