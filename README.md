# Deploy your WebApp to Azure App Service through Local Git.
## Summary: In this tutorial, you will learn how to deploy your AspNet Web App to Azure App Service using our Local git.
## Azure App Service
Azure App Service is a platform as a service (PAAS) offering from Microsoft Azure that allows you to deploy Webapps, Mobile backends, and Restful APIs in any programming language of your choice without managing infrastructure.

The following illustration shows the deployed application.

![image](https://github.com/user-attachments/assets/d8f845be-f9cb-4399-a1a5-ebe1fabd7478)

## Prerequisites

1. Visual Studio(Visual Studio Code)
2. .NET 8.0 LTS

We have the source code on this repository. The source code is a basic AspNet WebApi project so you could create one and use that for this tutorial.

Excersice 1: Create Azure App Service on Azure

Option 01. 
Sign in to your Azure account at https://portal.azure.com. If you do not already have one, create an account to get a $200 Azure credit. You’ll have 30days to use this credit in addition to free resources available on the portal.

Option 02. 
Sign in to your Azure account at https://portal.azure.com. You can use crome browser in Incognito mode.Go to google.com then search "Azure learning" then click browseAll then search "Azure web hosting" ..... You can learn more detail about this if you do not know this.

When signed in, Go to the App Service Deployment page. then click on create.
![image](https://github.com/user-attachments/assets/fbe12cb6-dbb9-4e74-a2ae-47a9f7ca5d06)

## Create Web App
![image](https://github.com/user-attachments/assets/2cba57c7-9e25-4523-838a-59e7e319b6cc)

Here app name "testdempapp"
## Deployment Center
![image](https://github.com/user-attachments/assets/e5c384f6-3689-4d24-9d57-00ed97c29d88)

#### Local Git/FTPS credentials
![image](https://github.com/user-attachments/assets/24ea1f45-eddc-414b-a956-ff5f57dca381)

#### Go to your local PC
![image](https://github.com/user-attachments/assets/9b863e74-a66b-4622-9d39-ccdf488ad3e2)

#### Open windows PowerShell
![image](https://github.com/user-attachments/assets/81599e64-64be-4162-8df8-c4281eb7a4ee)

1. PS F:\Practice Project\.NET 8.0\DemoDotNet8AppForAzureWebHostiog> git init
2. PS F:\Practice Project\.NET 8.0\DemoDotNet8AppForAzureWebHostiog> git add .
3. PS F:\Practice Project\.NET 8.0\DemoDotNet8AppForAzureWebHostiog> git commit -m "first"
4. PS F:\Practice Project\.NET 8.0\DemoDotNet8AppForAzureWebHostiog> git remote add azure https://testdempapp-fbhhcfd9csdngdg4.scm.eastus-01.azurewebsites.net:443/TestDempApp.git
5. PS F:\Practice Project\.NET 8.0\DemoDotNet8AppForAzureWebHostiog> git push -u azure master

![image](https://github.com/user-attachments/assets/f1edf832-6a88-498f-9b97-50125f639385)

remote: Deployment successful.

Go to your azure portal and check your application is deployed successfully.
