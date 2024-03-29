# Automated Infrastructure as Code (IaC) Deployment with Security Compliance

This project demonstrates the use of Terraform for Infrastructure as Code (IaC), Ansible for configuration management, and OpenSCAP for security compliance, integrated into a CI/CD pipeline. Showcasing automated, secure infrastructure deployment on GitHub.

![diagram (2)](https://github.com/danielamoh1/Automated-IaC-Deployment-with-Security-Compliance/assets/160555417/da9d4e54-4441-410e-9d03-120424954469)

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

[] **Initialize a new Git repository.**
   ```bash
   git init Automated-IaC-with-Security-Compliance
   cd Automated-IaC-with-Security-Compliance
   ```

######### Create the project structure. ###############
```bash
mkdir -p terraform ansible openscap .github/workflows
touch README.md terraform/{main.tf,variables.tf,outputs.tf} ansible/playbooks/main.yml
```
[] **Terraform Implementation**

Define your AWS infrastructure in terraform/main.tf.
Specify any necessary variables in terraform/variables.tf.
Define output variables in terraform/outputs.tf.

[] **Ansible Configuration**

Create Ansible playbooks in ansible/playbooks/.
Define roles for web, app, and database configurations in ansible/roles/.

[] **Security Compliance with OpenSCAP**

Add OpenSCAP scan definitions in the openscap/ directory.
Integrate OpenSCAP scans into the CI/CD pipeline for automated compliance verification.

[] **CI/CD Pipeline Configuration**

Configure GitHub Actions in .github/workflows/main.yml to automate:
Terraform deployment.
Ansible configurations.
OpenSCAP compliance scans.
