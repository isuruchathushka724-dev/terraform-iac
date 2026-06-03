# 🏗️ Terraform IaC — AWS EC2 & S3 Provisioning

> Automate AWS infrastructure deployment using Terraform. This project provisions an EC2 instance and an S3 bucket through reusable, version-controlled Infrastructure as Code — eliminating manual setup and ensuring consistent, repeatable environments.

![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white)
![HCL](https://img.shields.io/badge/HCL-844FBA?style=flat)

## 📋 Overview

Manually setting up cloud infrastructure is slow, error-prone, and hard to replicate. This project solves that by defining AWS resources as code, so the entire environment can be created, updated, or torn down with a single command — fully version-controlled and reusable across projects.

## 🛠️ Tech Stack

- **IaC Tool:** Terraform
- **Cloud Provider:** AWS
- **Resources:** EC2, S3
- **Language:** HCL

## 📁 Project Structure

```
terraform-iac/
├── main.tf       # Main infrastructure configuration
├── variables.tf  # Input variables
├── outputs.tf    # Output values
├── .gitignore    # Ignored files (state, secrets)
└── README.md     # Project documentation
```

## 🚀 Usage

```bash
# Clone the repo
git clone https://github.com/isuruchathushka724-dev/terraform-iac
cd terraform-iac

# Initialize Terraform
terraform init

# Preview changes
terraform plan

# Apply infrastructure
terraform apply

# Destroy when done (avoid charges)
terraform destroy
```

## ⚙️ Input Variables

| Variable        | Description        | Default                             |
| --------------- | ------------------ | ----------------------------------- |
| `aws_region`    | AWS region         | `us-east-1`                         |
| `ami_id`        | AMI ID for EC2     | `ami-0c02fb55956c7d316`             |
| `instance_type` | EC2 instance type  | `t2.micro`                          |
| `bucket_name`   | S3 bucket name     | `cv-project-terraform-bucket-isuru` |

## 📤 Outputs

| Output            | Description                    |
| ----------------- | ------------------------------ |
| `ec2_instance_id` | ID of the created EC2 instance |
| `ec2_public_ip`   | Public IP of the EC2 instance  |
| `s3_bucket_name`  | Name of the created S3 bucket  |

## ✅ Best Practices Used

- Sensitive files (`.tfstate`, credentials) excluded via `.gitignore`
- Configuration fully parameterized with variables for reusability
- Resources destroyed after demo to avoid AWS billing

## 👨‍💻 Author

**Isuru Chathushka** — Undergraduate @ Horizon Campus LK
🔗 [LinkedIn](https://www.linkedin.com/in/isuru-chathushka)
