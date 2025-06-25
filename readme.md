# AWS Cloud Migration Demo with Terraform

## Overview

This project demonstrates a simple cloud migration scenario using Terraform to provision AWS infrastructure. The goal is to simulate migrating an application environment from an on-premises setup to AWS cloud. It includes provisioning key AWS resources such as EC2 instances, networking components, and security groups.

## Purpose

The purpose of this demo is to showcase:
- How to define cloud infrastructure as code using Terraform
- Basic AWS resource provisioning to support application migration
- Infrastructure automation best practices
- A foundation for understanding cloud migration workflows and patterns

## Project Structure

- `main.tf` - Core Terraform configuration defining AWS resources
- `variables.tf` - Input variables to customize the deployment
- `outputs.tf` - Outputs showing key information after deployment
- `.gitignore` - Standard files to ignore in the repo

## Prerequisites

- Terraform installed (version >= 1.0)
- AWS CLI configured with appropriate credentials
- An active AWS account with permissions to create EC2, VPC, and related resources

## How to Use

1. Clone this repository  
   ```bash
   git clone https://github.com/yourusername/aws-cloud-migration-demo.git
   cd aws-cloud-migration-demo

2.  Initialize Terraform
terraform init

3. Review and customize variables in variables.tf as needed.

4. Plan the deployment
terraform plan

5. Apply the deployment
terraform apply

6. Once deployed, Terraform will output key resource information such as instance IP addresses.

7. To destroy the infrastructure after testing:
terraform destroy

Learning Outcomes
This demo helps you get hands-on experience with:

Writing Infrastructure as Code (IaC) using Terraform

Managing AWS cloud resources for migration projects

Automating deployments for repeatability and scalability

Notes
This is a simplified demo project for educational purposes and does not cover complex production scenarios like high availability, load balancing, or advanced networking.

# Cloud Migration Demo using Terraform & AWS

## 🔧 Infrastructure Overview (ASCII Diagram)

 [On-Prem App]
        |
        |   (Migration)
        v
+-----------------------+
|    AWS Cloud         |
|  ------------------  |
|  | EC2 Instance    |  | <-- Hosts the migrated app
|  |----------------|  |
|  | RDS (MySQL)    |  | <-- Stores application data
|  |----------------|  |
|  | S3 Bucket      |  | <-- Stores static assets/logs
|  ------------------  |
+-----------------------+
💡 This diagram reflects the core architecture of a typical on-prem to AWS cloud migration.

Why This Project Matters
This project demonstrates hands-on experience with:

Infrastructure as Code (IaC) using Terraform to provision cloud resources

Cloud migration best practices, moving legacy apps from on-prem to AWS

Real-world deployment patterns involving EC2, RDS, and S3

Knowledge of cloud models (IaaS, PaaS), AWS services, and DevOps mindset

Demonstrated project ownership, technical initiative, and deployment skills

Whether you're a hiring manager seeking someone who can hit the ground running in cloud projects, or a recruiter looking for strong foundational AWS + Terraform skills — this project shows capability in realistic enterprise cloud transformation work.

How to Run This Project Locally
Prerequisites:

Terraform installed: https://developer.hashicorp.com/terraform/downloads

AWS CLI installed and configured

An AWS account with programmatic access

Steps:
# Clone the repository
git clone https://github.com/yourusername/cloud-migration-demo.git
cd cloud-migration-demo/infrastructure

# Initialize Terraform
terraform init

# Preview changes
terraform plan

# Apply the infrastructure
terraform apply
🔐 You may need to customize variables (e.g., region, credentials) in the main.tf or terraform.tfvars.

Created by A Riley
