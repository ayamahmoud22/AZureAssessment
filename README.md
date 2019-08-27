# Azure Assessment using ARM Template

Using ARM template, created 2 Virtual Machines under an Internal Load balancer,also deploys a Storage Account, Virtual Network referencing a Public IP Address with 2 Network Interaces Cards In additonal to Availability Set.
Also, Deployed: App Service Plan, Web App,Storage account
The web application Idea is a photo Gallery hosts, views and deleles photos in URL : https://sentiaarm.azurewebsites.net/ from/in the storage account.


Deployment Steps:


1- Deployed the (App Service Plan, Web App,Storage account ) from Visual Studio Azure Resource Group.

![Settings Window](https://github.com/MicrosoftDocs/azure-docs/raw/master/articles/azure-resource-manager/media/vs-azure-tools-resource-groups-deployment-projects-create-deploy/create-project.png)

2- Selected "webApp" template from the Azure Resource Manager

![Settings Window](https://github.com/MicrosoftDocs/azure-docs/raw/master/articles/azure-resource-manager/media/vs-azure-tools-resource-groups-deployment-projects-create-deploy/select-project.png)

3- Customize Resource Manager template "Paramaters, Variables"
![Settings Window](https://i.ibb.co/yStrK4z/VS.png)

4- Deploy project to Azure
For the AzureRM module script, use Visual Studio:

On the shortcut menu of the deployment project node, choose Deploy > New.
![Settings Window](https://i.ibb.co/4K3XTNy/VCDeploy.png)

Then configure the targeted ResourceGroup
![Settings Window](https://i.ibb.co/vwJwb7k/VCDeploy2.png)

After deploying
![Settings Window](https://i.ibb.co/NstgQhy/Azure.png)


Now, deploy the  2 Virtual Machines under an Internal Load balancer,also deploys a Storage Account, Virtual Network referencing a Public IP Address with 2 Network Interaces Cards In additonal to Availability Set.

