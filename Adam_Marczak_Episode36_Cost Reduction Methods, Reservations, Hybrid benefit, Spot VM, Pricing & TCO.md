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

Imagine a scenario where in your on-premise data center, you have a virtual machine with one virtual core running Windows Server because this virtual machine is running Windows server that means you also purchased a license for a Windows Server for one core. When you migrate this workload to Azure, you will also create a virtual machine of the same size with one virtual core and you will pay the price for the compute power with one virtual core assigned.
