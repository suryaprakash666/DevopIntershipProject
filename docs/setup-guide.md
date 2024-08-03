# Setup Guide

## Prerequisites
Before starting, ensure you have the following:
- Azure account
- GitHub account
- SSH access to the Azure VM
- Maven installed on the VM
- Jenkins installed on the VM
- Tomcat installed on the VM

## Step-by-Step Instructions

### 1. Setting up Azure VM
1. Log in to your Azure account:
   - Go to [Azure Portal](https://portal.azure.com/).

2. Create a new Resource Group:
   - Navigate to "Resource Groups".
   - Click "Add" and provide a name and region for the resource group.
   - Click "Review + Create" and then "Create".

3. **Create a new Virtual Machine within the Resource Group:
   - Navigate to "Virtual Machines".
   - Click "Add" and select the resource group you created.
   - Provide a name for the VM, choose "Redhat Linux" as the OS, and select a size (Standard B1s or appropriate size).
   - For "Authentication type", select "SSH public key" and paste your public key.
   - Configure network settings to allow SSH, HTTP, and HTTPS traffic.
   - Click "Review + Create" and then "Create".

### 2. Installing and Configuring Tools

#### 2.1 SSH into the VM
Open your terminal and connect to the VM using SSH:
"ssh your_username@your_vm_ip_address"
