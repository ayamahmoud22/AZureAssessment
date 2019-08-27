## Azure Assessment using ARM Template

Using ARM template, created 2 Virtual Machines under an Internal Load balancer,also deploys a Storage Account, Virtual Network referencing a Public IP Address with 2 Network Interaces Cards In additonal to Availability Set.
Also, Deployed: App Service Plan, Web App,Storage account
The web application Idea is a photo Gallery hosts, views and deleles photos in URL : https://sentiaarm.azurewebsites.net/ from/in the storage account.


##Deployment Steps##


*1- Deployed the (App Service Plan, Web App,Storage account ) from Visual Studio Azure Resource Group.*

![Settings Window](https://github.com/MicrosoftDocs/azure-docs/raw/master/articles/azure-resource-manager/media/vs-azure-tools-resource-groups-deployment-projects-create-deploy/create-project.png)

*2- Selected "webApp" template from the Azure Resource Manager*

![Settings Window](https://github.com/MicrosoftDocs/azure-docs/raw/master/articles/azure-resource-manager/media/vs-azure-tools-resource-groups-deployment-projects-create-deploy/select-project.png)

*3- Customize Resource Manager template "Paramaters, Variables"*
![Settings Window](https://i.ibb.co/yStrK4z/VS.png)


Using the Publish Website dialog, select Microsoft Azure Web Apps

In the next dialog, either select an existing web app, or follow the prompts to create a new web application. Note: If you choose to create a web application, the Web App Name chosen must be globally unique.

Once you have selected the web app, click Publish

*4- Deploy project to Azure*
For the AzureRM module script, use Visual Studio:

On the shortcut menu of the deployment project node, choose Deploy > New.

Then configure the targeted ResourceGroup
![Settings Window](https://i.ibb.co/vwJwb7k/VCDeploy2.png)

After deploying
![Settings Window](https://i.ibb.co/NstgQhy/Azure.png)


*5- In the Web.config file of the custom "Photo Album" webApp, located in the project root, edited the StorageConnectionString app setting and replace the placeholder values with the values obtained in the StorageAccount just been created.*

In Visual Studio Solution Explorer, right-click on the project name and select Publish...
![Settings Window](https://i.ibb.co/JCLNzZy/App-Con-String.png)


**Now, deploy the  2 Virtual Machines under an Internal Load balancer,also deploys a Storage Account, Virtual Network referencing a Public IP Address with 2 Network Interaces Cards In additonal to Availability Set.**

Edited the ARM template with the needed parameters with the public IP, NSG then deploy it in the portal

![Settings Window](https://i.ibb.co/mzQmbs4/Portal-ARM.png)


***After successful deployment***
![Settings Window](https://i.ibb.co/BsYP1Dr/AzureRG.png)
