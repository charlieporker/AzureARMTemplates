# Azure vNet with 3 subnets and NSG template

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.github.com%2Fcharlieporker%2FAzureARMTemplates%2Flob%2Fmaster%2FvNet3Subnets%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.github.com%2Fcharlieporker%2FAzureARMTemplates%2Flob%2Fmaster%2FvNet3Subnets%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Table of Contents

1. [Overview](#overview)
2. [Important Notes](#importantnotes)
3. [Pre Deployment Steps](#predeployment)
4. [Deployment](#deployment)
5. [Post Deployment Steps](#postdeployment)
6. [Teardown Deployment](#teardown)
7. [References](#references)

<a name="overview"></a>

## Overview
This template provisions an Azure VNET with 3 Subnets and NSG groups.

<a name="importantnotes"></a>

### Important Notes

* Do not run this solution in a **production environment/subscription**.
* It is recommended you use a clean Windows 10 (or similar) VM to perform the solution to ensure that the correct PowerShell modules get loaded.
* Deployment takes around **40-45 minutes** to complete.

<a name="predeployment"></a>

### Pre Deployment Step

Before proceeding to the deployment of the template, we need to perform the following steps.

**Note:** You can perform these steps through the Azure portal as well.

#### 1. Install the required Powershell modules

* Install and configure the Azure PowerShell module

    Follow the instructions in the article to [install the Azure PowerShell module and connect to your Azure subscription](https://docs.microsoft.com/powershell/azure/install-azurerm-ps?toc=%2fazure%2factive-directory-domain-services%2ftoc.json).

#### 2. Connect To Azure 

    # Connect to your Azure Account.
    Add-AzureRmAccount

<a name="deployment"></a>

<p></p>

**Note:** 
* Deployment takes around 5 minutes

<a name="postdeployment"></a>

### Post Deployment Steps

#### 1. Check vNet and Subnets in Azure Portal
To check configuration status:
Go to the Azure portal -> Select Network resource group -> Click vNet -> Review Subnets

<a name="teardown"></a>

### Teardown Deployment
To remove this deployment simply remove the resource group that contains this sample. 
    
<a name="references"></a>

### References
1. Pre-requisites: https://docs.microsoft.com/en-us/azure/active-directory-domain-services/active-directory-ds-enable-using-powershell
