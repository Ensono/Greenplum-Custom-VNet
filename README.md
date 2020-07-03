# Greenplum-Custom-VNet
The [Azure Marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/pivotal.pivotal-greenplum-azure-byol?tab=Overview) version of Greenplum does not have the option to create the service with an existing virtual network. The template mandates the creation of a new virtual network. This modifies the marketplace template from Pivitol enabling deployment to an existing virtual network.

## Prerequisites
1. Existing virtual network and subnet
2. Approporiate permissions (see section below)

## Permissions
The template provides the master virtual machine created in the template with Contributor rights to the resource group in order to shut down slave nodes in the cluster. So when deploying, you must ensure you have an appropriate role on your account to modify permissions.