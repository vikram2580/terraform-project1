# Azure Infrastructure Automation with Terraform – Project 1

This project demonstrates end-to-end Azure infrastructure provisioning using **Terraform** with a modular and reusable design approach.

## 🚀 Architecture Overview

The infrastructure includes:
- Azure Resource Group
- Virtual Network with custom address space
- Subnet with Network Security Group (NSG)
- Linux and Windows Virtual Machines
- Availability Sets for high availability
- Azure Storage Account
- Log Analytics Workspace
- Recovery Services Vault
- Azure Monitor & Network Watcher extensions

## 🛠 Technologies Used
- Terraform
- Microsoft Azure
- Azure Virtual Machines (Linux & Windows)
- Azure Networking (VNet, Subnet, NSG)
- Azure Monitor & Log Analytics
- Azure Recovery Services

## 📁 Project Structure
├── modules/
│ ├── rgroup-n01718323
│ ├── network-n01718323
│ ├── common-n01718323
│ ├── vmlinux-n01718323
│ └── vmwindows-n01718323
├── main.tf
├── variables.tf
├── outputs.tf


## ⚙️ Key Features
- Modular Terraform architecture for reusability
- Automated provisioning of multiple Linux VMs using `for_each`
- High availability using Availability Sets
- Secure networking using NSGs
- Monitoring enabled with Azure Monitor Agent
- Boot diagnostics enabled via Azure Storage

## ▶️ How to Deploy
```bash
terraform init
terraform validate
terraform plan
terraform apply
