Using this template, network security group can be deployed.

->To deploy a template, sign in to either the Azure CLI or Azure PowerShell

     az login
     
->Create a resource group

     az group create --name resourceGroupName --location "West Europe"
     
->Deploy template

     az deployment group create --name DeployLocalTemplate --resource-group $resourceGroupName --template-file <PATH-TO-multiplestorage.JSON> --parameters <PATH-TO-multiplestorage.PARAMETERS.JSON> 
