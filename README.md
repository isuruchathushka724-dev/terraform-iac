# 🏗️ Terraform IaC — AWS EC2 & S3 Provisioning

Infrastructure as Code project provisioning AWS EC2 
instances and S3 buckets using Terraform.

## 🛠️ Tech Stack
- **IaC Tool:** Terraform
- **Cloud Provider:** AWS
- **Resources:** EC2, S3
- **Language:** HCL

## 📁 Project Structure
terraform-iac/
├── main.tf          # Main infrastructure config
├── variables.tf     # Input variables
├── outputs.tf       # Output values
└── .gitignore       # Ignored files

## 🚀 Usage
```bash
# Clone repo
git clone https://github.com/isuruchathushka724-dev/terraform-iac
cd terraform-iac

# Initialize Terraform
terraform init

# Preview changes
terraform plan

# Apply infrastructure
terraform apply

# Destroy when done
terraform destroy
```

## ⚙️ Variables
| Variable | Description |
|----------|-------------|
| `aws_region` | AWS region to deploy |
| `instance_type` | EC2 instance type |
| `bucket_name` | S3 bucket name |

## 👨‍💻 Author
**Isuru Chathushka** | Undergraduate @ Horizon Campus LK  
[LinkedIn](https://www.linkedin.com/in/isuru-chathushka)
