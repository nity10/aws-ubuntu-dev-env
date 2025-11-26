# aws-ubuntu-dev-env
Project 2: Cloud Development Environment (Git &amp; Ubuntu)
☁️ Ubuntu Cloud Development Environment Setup

## 📌 Project Overview
This project focuses on setting up a remote development environment using **Ubuntu 22.04 LTS** on AWS. It involves system hardening, package management updates, and the configuration of **Git** for distributed version control.

## 🛠 Tech Stack
- **OS:** Ubuntu 22.04 LTS (Jammy Jellyfish)
- **Version Control:** Git 2.34.1
- **Remote Access:** SSH

## ⚙️ Implementation Steps

### 1. Environment Setup
- Deployed an Ubuntu Server instance on AWS.
- Established a secure SSH connection to the remote Linux terminal.

### 2. Package Management & Tooling
Unlike Amazon Linux (which uses `yum`), Ubuntu uses `apt`. I executed the following workflow to prepare the environment:

```bash
# 1. Update the local package index
sudo apt update

# 2. Install Git
sudo apt install git -y

# 3. Verify Git installation
git --version
