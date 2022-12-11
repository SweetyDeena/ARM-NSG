Using this template, network security group can be deployed.

->To deploy a template, sign in to either the Azure CLI or Azure PowerShell

     az login
     
->Create a resource group

     az group create --name resourceGroupName --location "West US"
     
->Deploy template

     az deployment group create --name DeployLocalTemplate --resource-group $resourceGroupName --template-file <PATH-TO-nsg.JSON> --parameters <PATH-TO-nsg.PARAMETERS.JSON> 
