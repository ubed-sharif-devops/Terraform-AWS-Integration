# AWS Infrastructure as Code (IaC) with Terraform

This repository contains modular Terraform code to provision and manage highly available, scalable AWS cloud infrastructure following Security and DevOps best practices.

## Architecture Highlights
- **Networking:** Multi-AZ VPC with Public/Private Subnets, NAT Gateways, and Route Tables.
- **Compute & Containers:** Amazon ECS / EKS clusters with auto-scaling node groups.
- **Security:** IAM Roles, Least-Privilege Policies, and Security Groups.
- **State Management:** Remote S3 Backend with DynamoDB state locking.

## Prerequisites
- [Terraform CLI](https://developer.hashicorp.com/terraform/downloads) (>= 1.5.0)
- [AWS CLI](https://aws.amazon.com/cli/) configured with proper credentials
- Git

## Repository Structure
- `modules/`: Contains reusable, parameterizable Terraform modules.
- `environments/`: Contains environment-specific declarations (`dev`, `prod`).

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/aws-terraform-infrastructure.git
   cd aws-terraform-infrastructure/environments/dev
