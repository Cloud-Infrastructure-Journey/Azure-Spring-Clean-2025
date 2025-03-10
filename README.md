# Azure Spring Clean 2025 - The Future of AKS Monitoring: Trends and Tools You Can’t Ignore

## Azure AKS Monitoring with Azure Monitor

This guide provides an overview of how to monitor Azure Kubernetes Service (AKS) using Azure Monitor, integrate with Azure Managed Grafana, and set up Azure Alerts with Azure Monitor recording and alert rules.

<img src="images/azure-spring-clean-2025-AKS-diagram.png" width="600" alt="AKS Monitoring" />

## Prerequisites

- Active Azure subscription
- AKS cluster
- Azure CLI installed
- Azure Monitor workspace
- Azure Managed Grafana instance

To deploy Azure AKS Monitoring using the Bicep files in the folder, follow the following steps:

## Deployment Steps

1. **Create a Resource Group**:
   ```sh
   az group create --name aks-mon-rg --location northeurope
   ```

2. **Deploy the Bicep File**:
   ```sh
   az group deployment create --resource-group aks-mon-rg --template-file aks-manged-prom.bicep --parameters location=northeurope name=aks-mon-cluster
   ```

3. **Clean Up Resources** (optional):
   ```sh
   az group delete --name aks-mon-rg
   ```

These steps will help you set up Azure AKS Monitoring with Azure Monitor, Azure Managed Grafana, and Azure Alerts using the provided Bicep files.
