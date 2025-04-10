# Azure Infrastructure as Code Deployment

This repository contains ARM templates and deployment scripts for provisioning Azure infrastructure with best practices.

## Resources Deployed

- App Service with VNET integration
- App Service Plan (Linux)
- Virtual Network with dedicated subnet for App Service
- Network security configurations

## Deployment Options

### 1. Deploy to Azure Button

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsarangvishnu%2Ffioneer-demo%2Fmain%2Ftemplates%2FmainTemplate.json)

### 2. GitHub Actions

The repository includes GitHub Actions workflows that automatically validate and deploy changes when pushed to the `main` branch.

### 3. Local PowerShell Deployment

```powershell
# For development environment
.\scripts\deploy.ps1 -Environment dev

# For production environment
.\scripts\deploy.ps1 -Environment prod
