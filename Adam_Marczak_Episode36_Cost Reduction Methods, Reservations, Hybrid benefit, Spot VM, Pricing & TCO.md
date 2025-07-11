# AZ-900 Episode 36 | Cost Reduction Methods, Reservations, Hybrid benefit, Spot VM, Pricing & TCO

We will learn multiple ways to reduce the cost of our Azure services. We will also discover two tools: **pricing** and **TCO calculator**

![image](https://github.com/user-attachments/assets/0221adea-fc4e-482a-b890-8097e694cf76)

## Reservations

In Azure, you purchase capacity of the services overtime. In case of virtual machine, this simply means performance and one of the biggest ebenfits of the cloud is being able to shut this virtual machine down whenever you don't need it, turn it ON when you need it, or even cale up and down whenever that's necessary. The best part is you will only pay for the usage. The **usage** means the cost of the service. 
What happens if you have a different kind of workload?
A Workload that does not need those benefits of the cloud, a very stable workload that will constantly consume one virtual core of that virtual machine over time and you won't be shutting it down or scaling up this virtual machine therefore you're losing those benefits of the cloud. Does that mean you have no way to reduce the cost of that virtual machine?
There's a way by using **Azure Reservations**. 

Let's say we purcahse a virtual machine with one virtual core and this virtual machine price is $50/month. If you buy that virtual machine and you will use it for one week, this will cost you $12, if you purchase that for one month it will be $50. If you will use that virtual machine throughout the year, it will cost you $600. If you know you will be using it for this long period of one year, what if you could reserve that virtual machine and get a discount for that. If you do it and you reserve that capacity if you will  commit yourself to that one virtual core capacity of that virtual machine for an entire year, Microsoft will give you a discount. The cost of this virtual machine will suddenly drop to $360 a year. By that, the cost of our virtual machine per month drops to $30. That means we're getting 40% discount but reservations can also be made for longer period of three years. In this case, you would pay $720 for 3 years of that virtual machine making it only $20 per month or 60% discount of the total price. 

<img width="925" height="509" alt="image" src="https://github.com/user-attachments/assets/74386ecb-f454-4159-94b9-50b428b1567e" />

### There are three types of **Reservations** that you can make in Azure.

1. **Reserved Instances** meaning that you reserve the virtual machine performance where you reserve the SKU, the compute power of your virtual machines.

2. You can also **Reserved Capacity** for Platform as a Service (PaaS) offerings like Azure storage, SQL Database, Databricks Units (DBUs), Cosmos DB, RUs, etc, ect

3. Besides that, you can also make reservations for **software plans**. At this point in time, this means reserving the licensing costs for operating systems like Red Hat.


Just remember that those reservations are made for one or three year periods. 

<img width="873" height="407" alt="image" src="https://github.com/user-attachments/assets/5f9a70b4-e60a-433b-b91d-206dea666f83" />


# Spot VM

<img width="450" height="495" alt="image" src="https://github.com/user-attachments/assets/7953d162-2b60-4fc2-8bad-cb1967d9fa18" />

Imagine this box represents the data center capacity for virtual machines. When customers purchase virtual machines, certain part of that capacity is being used. At the same time, Microsoft needs to be able to have a lot of unused capacity in order to meet growing demand and those auto-scaling features of the cloud. So they need to have a reserve of the capacity whenever customers need it. Wouldn't it be awesome if you could use that unused capacity at the discount? You can and this is exactly what **Spot Virtual Machines** are. You can buy that unused capacity at a significant discount. If Microsoft will need that capacity back, they can take it at any time. 

Depending on the capacity that is left in the data center, you will get a different discount. If there's a very little capacity that is being unused, the discount will be very low therefore the price of the spot VM will increase. If there's a lot of unused capacity, the discount will be very high therefore your cost will be very low.

<img width="450" height="266" alt="image" src="https://github.com/user-attachments/assets/36221b30-16eb-4a63-a24b-388913693d76" />


<img width="882" height="483" alt="image" src="https://github.com/user-attachments/assets/0262d5b8-8a58-45d5-bc05-93045dd0738a" />


# Hybrid Use Benefit

Imagine a scenario where in your on-premise data center, you have a virtual machine with one virtual core running Windows Server because this virtual machine is running Windows server that means you also purchased a license for a Windows Server for one core. When you migrate this workload to Azure, you will also create a virtual machine of the same size with one virtual core and you will pay the price for the compute power with one virtual core assigned because this virtual machine is using Windows, you will also need to choose Windows virtual machine in Azure therefore your price for virtual machine will also include the cost of the license. 
When you go to any kind of calculator in Azure, you will quickly notice that the price for Windows machines is always higher than when comparing those to a Linux machine. This is because a Linux like Ubuntu is free whereas for Windows, you need to pay for the Windows server licenses but in this scenario, you already have the license for your Windows server and then you're paying additionally the cost of the licensing cloud that doesn't  make sense.
**This is where hybrid use comes into play.**
You can use this license in the cloud by selecting hybrid benefit when you create your virtual machine.
When you do it, it will remove the cost of the license associated with the virtual machine therefor the cost of your virtual machine will be only associated with the compute power.
If you combine the hybrid use benefit with Azure reservations, you can significantly reduce the cost of your Azure environments.

<img width="805" height="509" alt="image" src="https://github.com/user-attachments/assets/0a54b4f3-7f56-458d-908e-fb454f07c5bd" />

Hybrid benefits allows you to use exisiting licenses that you already purchased for Windows Server, RedHat, SUSE, or SQL Server in Azure.

For the first three, we're talking about the operating costs on other virtual machines but when it comes to SQL server you can significantly reduce the price of Azure SQL databases. Azure SQL managed instances, SQL server on virtual machine and even data factory running SQL

<img width="649" height="441" alt="image" src="https://github.com/user-attachments/assets/181ddf59-759c-42c0-bd03-957c4d8de71b" />


### Cost Reduction Methods

There are two tools that we need to mention when it comes to cost reduction. Those are **Azure pricing calculator** which we already saw in the previous episode. In this pricing calculator, you choose the service that you want to use then you adjust the variables, the parameters for the service, and you review the cost.

Let me show you how this works with one 

<img width="790" height="306" alt="image" src="https://github.com/user-attachments/assets/b56ff58c-c185-4c84-9a53-b730d5b54a50" />

Second tool is called **Total Cost of Ownership (TCO) Calculator**. It allows you to compare the cost of running certain workloads in your data center versus Azure. The process is also very simple, first, you define your workloads that you have in your datacenter then you adjust some assumptions like the cost of labor, cost of the licenses, adjust what kind of things you would want to leverage in Azure.

Then you are presented with a report which shows you the comparison of running that particular workload in Azure versus your own data center.

<img width="829" height="491" alt="image" src="https://github.com/user-attachments/assets/c1cfbf96-75ec-462c-9395-c29d7e094489" />


<img width="1305" height="632" alt="image" src="https://github.com/user-attachments/assets/7c0be6b5-9622-466a-9ac4-533e9c9f5f94" />

