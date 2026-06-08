# GCP Cloud Run Serverless Studio

This repository contains the target configuration and SRE runtime files compiled by the **GCP Cloud Run Serverless Studio** dashboard module.

## 🚀 Description
Configure serverless container applications on Google Cloud Run. Generate service definitions, VPC connectors, custom Domain mappings, and scaling limits configs.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/run/cloud_run.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-gcp-cloud-run.git
   cd tp-gcp-cloud-run
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
