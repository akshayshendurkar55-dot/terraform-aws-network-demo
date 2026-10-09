# Terraform AWS Network Demo

A hands-on Infrastructure as Code (IaC) project demonstrating how to provision an AWS Virtual Private Cloud (VPC) and a public subnet using Terraform.

## Project Overview

This project introduces the fundamentals of AWS networking through Terraform configuration. It focuses on creating a custom VPC and public subnet while practicing reusable variables, resource outputs, and the Terraform workflow.

## Architecture

```text
AWS
└── VPC
    └── Public Subnet
```

**Note:** A public subnet typically requires an appropriate route to an Internet Gateway and suitable network configuration for internet connectivity. This project focuses on the VPC and subnet resources.

## Technologies Used

* Amazon VPC
* AWS Subnets
* Terraform
* Git and GitHub

## Features

* Custom VPC provisioning
* Public subnet provisioning
* Reusable configuration through Terraform variables
* Outputs for VPC and subnet IDs
* Infrastructure planning and validation using Terraform

## Repository Structure

```text
terraform-aws-network-demo/
├── .gitignore
├── .terraform.lock.hcl
├── README.md
├── main.tf
├── variables.tf
└── outputs.tf
```

## Prerequisites

* Terraform CLI
* AWS CLI
* An AWS account with appropriately configured credentials
* IAM permissions required for the resources in this project

Never commit AWS access keys or secret credentials to GitHub.

## Terraform Workflow

### 1. Clone the repository

```bash
git clone https://github.com/akshayshendurkar55-dot/terraform-aws-network-demo.git
cd terraform-aws-network-demo
```

### 2. Initialize Terraform

```bash
terraform init
```

### 3. Format and validate

```bash
terraform fmt
terraform validate
```

### 4. Review the plan

```bash
terraform plan
```

Inspect the planned resources before deciding whether to deploy.

### 5. Apply the configuration

```bash
terraform apply
```

Only proceed after reviewing the plan and considering potential AWS charges.

### 6. View outputs

```bash
terraform output
```

The configured outputs can display the VPC ID and subnet ID after a successful deployment.

## Cost and Cleanup

AWS resources may incur charges depending on the resource type, region, and current pricing. Review the AWS Billing dashboard and the resources Terraform plans to create.

When you have finished testing, verify that it is safe to remove the resources managed by this configuration, then run:

```bash
terraform destroy
```

Review the destruction plan before confirming. Check the AWS Console afterwards for any remaining resources or charges.

## Learning Outcomes

* Understanding VPC and subnet fundamentals
* Defining AWS networking resources with Terraform
* Practicing variables and outputs
* Using the Terraform init, validate, plan, apply, and destroy workflow
* Considering cost and cleanup when working with cloud infrastructure

## Author

**Laxmikant Shendurkar**

Cloud Computing and DevOps Learning Projects
