# Automated Infrastructure as Code (IaC) Deployment with Security Compliance

This project demonstrates the use of Terraform for Infrastructure as Code (IaC), Ansible for configuration management, and OpenSCAP for security compliance, integrated into a CI/CD pipeline. Showcasing automated, secure infrastructure deployment on GitHub.

## Project Structure

- **README.md**: Project documentation.
- **terraform/**: Contains Terraform configurations for AWS resources.
  - **main.tf**: Main Terraform configuration file.
  - **variables.tf**: Terraform variables.
  - **outputs.tf**: Terraform outputs.
- **ansible/**: Ansible playbooks and roles.
  - **playbooks/**: Ansible playbooks for configuring EC2 instances.
  - **roles/**: Reusable Ansible roles for specific configurations.
- **openscap/**: OpenSCAP scan definitions and policies.
- **.github/workflows/**: CI/CD pipeline configurations for GitHub Actions.

## Step-by-Step Guide

### 1. Project Setup

1. Initialize a new Git repository.
   ```bash
   git init Automated-IaC-with-Security-Compliance
   cd Automated-IaC-with-Security-Compliance
   ```
