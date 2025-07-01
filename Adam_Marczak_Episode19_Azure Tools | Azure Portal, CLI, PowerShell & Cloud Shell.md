![image](https://github.com/user-attachments/assets/0a0140ed-3141-43bf-82ab-55a69613f206)

## Azure Portal

![image](https://github.com/user-attachments/assets/049b88ce-db9b-4fd6-b6e7-0bba0cc11829)

This is our web-interface, a publicly accessible web-interface for management of everything related to Azure platform.
It is designed for self-service, so all of the tasks are pretty easy to do.
99% of the things with azure can be done in Azure portal.
It is quite customizable because you can create your own dashboards to get a quick glance at your Azure resources and their statuses but what is important is Azure portal is designed to help customers with fairly simple tasks.
**It is not a tool that you will use if you want to do big deployments or automation tasks which brings us to Azure PowerShell**

## Azure PowerShell

Tool that allows us to automate stuff in Azure. Besides the classis approach of using browser and accessing Azure through Azure portal, you can also access Azure through a terminal. This works for both Windows, Linux, and MacOS. 
Just need to install PowerShell modules and you will be able to connect to Azure to work with Azure resources through a command terminal. This is one of the ways of managing Azure resources in an imperative way

![image](https://github.com/user-attachments/assets/5ef60d30-ab53-438e-b0ab-00b5d49a252a)

### Characteristics
- Azure PowerShell is simply a module that Microsoft created for a popular PowerShell scripting language
- It was designed to help with Automation tasks when it comes to Azure. With this module and PowerShell language, you can create very complex logic using scripts
- With the release of PowerShell core in 2016, you can now use PowerShell in any operating system- Windows, linux, MacOS
- It is simple to use. For example, you can type **connect-AzAccount** to login to Azure. You can also type **Get-AzResourceGroup** to list all the available resource groups in your Azure subscription. You can type **New-AzResourceGroup** if you want to create new resource groups. Type **New-AzVm** to create new virtual machine.
- Using those commands and very powerful scripting language which is PowerShell, you can create almost any automation tasks in no time
- You can then grab those scripts and either automate them in Azure or in a tool like Azure DevOps

![image](https://github.com/user-attachments/assets/462acd42-0fbf-4b86-bfa3-64632dd98794)

**PowerShell in general is a very native approach for IT professionals who are working with Windows Servers in the past but if your background is more on the Linux side, you might prefer to use **Azure CLI** instead**
 


## Azure CLI

Just like with PowerShell, you wil use terminal to log into Azure and manage Azure resources but instead of installing modules for PowerShell, you will install CLI. It is just another way of managing Azure resources through terminal

![image](https://github.com/user-attachments/assets/79c1fc06-d4d7-4d30-a8be-f3fbe2ee871c)


### Characteristics

![image](https://github.com/user-attachments/assets/99d96e8a-87ae-4d0b-8b20-973567485724)

- In short, Azure CLI is our command line interface for Azure
- It is also designed for automation just like PowerShell
- It is multi-platform- it's based on Python. You can use it on any operating system.
- Similarly to PowerShell as well, it is fairly simple to use because you just type **Az login** to log into Azure, **az group list** to list resource group, **az group create** to create new ones, or **az vm create** to create virtual machine

One important thing to note is that CLI is just a tool for the native terminal so depending on which Operating System terminal you are using, you will have different scripting capabilities so it's quite important decision to make here. In general, you can use either PowerShell or CLI to perform most of the tasks when it comes to Azure but its just a matter of preference. Microsoft wanted to provide you with toolkit so that you can use your existing skills whether you are coming from Windows or more Unix-based environments and integrate with Azure in no time which brings us to our last tool, **Azure Cloud Shell**

## Azure Cloud Shell

Everything we've talked about on this episode is happening on user machine. So users need to use their own browsers or they need to install tools like PowerShell or CLI to perform automations with Azure. There are many scenarios where you simply won't be able to install those tools locally or you don't have access to user machine on a specific time. Microsoft wanted to solve those challenges by providing another environment where all the tools will be pre-installed for you and will always be up-to-date. This extra environment is called **cloud shell**. You can access this through many interfaces. For example, through a web browser by navigating to **shell.azure.com**. There are a lot of cool things about cloud shell environment. For example, it's based on Ubuntu container so you get a lot of additional tools that come with Linux natively. You can use both PowerShell and CLI depending on which you prefer.
What's better, this environment is completely free. So you can perform your day-to-day operations directly from the browser without the need to install a single tool on your local machine.
Azure cloud shell also comes with a lot of interfaces to use it. You can use it from dedicated shell.azure.com portal, you can also use portal.azure.com with a small integration directly in Azure portal or if you are on the go and you don't have access to your machine or you don't want to open this, you can use mobile application which has a native integration with cloud shell

![image](https://github.com/user-attachments/assets/21e00229-40e6-41be-adfc-a81bbc7e7949)


### Characteristics

![image](https://github.com/user-attachments/assets/1769c93d-664f-4297-ba9b-42e8c6cea50d)

- **Azure Cloud Shell** is cloud-based scripting environment which is completely free to use and allows us to use both PowerShell and CLI directly in our browsers to connect to Azure and manage other resources.
- It has a lot of additional tools installed because it is based on Ubuntu machine
- A lot of client interfaces, you can use Azure portal (portal.azure.com), dedicated portal like shell.azure.com, you can also use visual studio code extension to connect to cloud shell directly from Visual Studio code, you can use Windows terminal, Azure mobile application, or use cloud directly in Microsoft Documentation when you are learning which is also one of the amazing features of cloud shell.

![image](https://github.com/user-attachments/assets/18a220e1-4629-40d2-bf47-eae2b85a9e74)


![image](https://github.com/user-attachments/assets/f270c25e-ea29-4a6e-8dcf-51d0ad83e9c9)


## Summary of Azure Tools discussed today

- **Azure portal**, our web-based interface for managing Azure platform
- **Azure CLI**, one of the automation tools for managing Azure resources through terminal
- If we want to create scripting using PowerShell, we can simply install Azure module and use PowerShell instead. This is just one of the multiple options available to us
- Lastly, we've learned about the cloud environemnt for scripting which is **Cloud Shell** to perform our day-to-day operations without a need to install anything on our local machines

![image](https://github.com/user-attachments/assets/bccfbe24-5c97-4421-a80f-6865c1980533)
