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
 
