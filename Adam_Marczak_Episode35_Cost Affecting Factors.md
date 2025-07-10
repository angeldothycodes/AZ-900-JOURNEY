We will learn about the key factors that affect the cost of your Azure services.

![image](https://github.com/user-attachments/assets/51e0a9c5-8bbd-4107-b729-196177004a4b)

Please note that the above are not the only cost affecting factors. But these four will be the key element that will drive the cost of your Azure environment.

# Resource Types

Resource types is simply the answer to the question **what kind service do we use?** When you buy a virtual machine in Azure, there are certain metrics that track the usage of your virtual machine resource.
For example when you choose what kind of **virtual machine** you want, you specify how much CPU, how much processor, how many cores, how much memory you want to have. Those metrics are tracked against the uptime. For how long did you have that virtual machine with this kind of configuration.
When you buy an **SQL database in Azure**, metrics are very similar there. You pay for processor, memory, additionally you pay for storage and then it's tracked against the uptime. How much storage, how much memory and CPU you used for how long. 
There are other services with much more flexible pricing models like **Azure functions** for instance. It's a service that allows us to execute small pieces of code and only pay for that. You pay for how many times did you execute your pieces of code and how much memory did those executions consume. 
But if you bought **Azure storage account** for instance, the price consists of how much storage you are consuming, what is the access tier for this data and how many operations are you doing on the storage account.

In the case of **Azure logic apps**, the pricing is even simpler. How many actions did you execute. 

One thing to note is resources that are only organizational resources and logical resources like **Resource groups** are free because they are not servers, they are logical objects in Azure. Those do not have any kind of cost associated.

What you should remember from this slide is that every resource type have a small metric that is tracking its usage and this will be your key factor that will affect the final cost of your Azure environment. Therefore you should always spend time to think what kind of use case do you have. What kind of application are you building and which are the right resource types for you.

![image](https://github.com/user-attachments/assets/b04d67dd-2b1b-42b3-b62e-8cb33724b928)

# Services

Beside resource types be aware that different service offerings of Azure have different price of services associated with them. When talking about services we're talking about **what kind of Azure offer do you have?**, **how did you purchase your Azure?**. As a customer, you have multiple ways to buy Azure from Microsoft.
One of the most common ways is buying this through a web portal wher you can get one of many available Azure offer types like **Azure Free** which is great for testing or **Pay-as-you-go** subscription where you are billed monthly for your Azure usage. You can also get some Azure credits from **Microsoft partner network** or if you have a visual studio license. There's plenty different offer types that you can choose from. 

Besides that you can contact Microsoft representative and buy an enterprise agreement. This is agreement between your company and Microsoft. This is a contract that you sign. Lastly, you can buy Azure from a partner of Microsoft so-called **Cloud Solution Providers**. This model in short is called CSP. So depending on which Azure offer type do you have, it will affect two things. One of them is **usage rate**, simply the cost of your **Azure services** and the billing cycle but the usage rates are changing because when you are purchasing Azure from an enterprise agreement or through CSP, you can negotiate the prices. If you negotiate any discounts, this discount will be applied for all the services available in your azure subscriptions. This will definitely affect the final cost of your Azure environment

![image](https://github.com/user-attachments/assets/27ec444a-5daf-4db6-96f1-f94fac168ad2)


# Location

There is one more very important thing when purchasing Azure services. This is the location of services. In which Azure region are our services currently located.

Let's imagine a scenario where you purchase Azure virtual machine in West Europe region. That virtual machine will have one virtual core and four gigabytes of memory. If you go to Azure pricing calculator, you might see that this virtual machine will cost you 100 US dollar per month but if you suddenly change region and you will pick exactly same machine with exactly same configuration in North Europe, you might see that the price suddenly differs. This is the exact same configuration, exact same resource type on exact same offer yet the price differs. You will see that across many different regions in Azure that as soon as you will start picking the same service but in different regions price will be different. The true answer is a little bit more complex but we can narrow it down to a simple statement that the cost of running Azure data center differs from region to region. 
My advice is that when you are picking the region for your Azure solution, pick the region that is nearby to your customers so the latency is small. The region that has all the services that you want to use and the lowest price for those services.


# Bandwidth/ Traffic

The last factor that affects the cost of your Azure environment is bandwidth. How much data are we moving to Azure and out of Azure?
When you are customers, the first thing that you will do most of the time is migrate to Azure. Therefore, in your company from your servers you will want to upload data to Azure Data Center. This upload is called **ingress** or otherwise called **inbound traffic**.
This is the **in** traffic from the perspective of Azure. This is incoming data to Azure data center. If you're downloading data from Azure, then we're talking about the **egress** or so-called **outbound traffic** because this is the traffic going out of Azure. What it should be noted is that most of the time, in most scenarios, **the traffic that is going to Azure is free**. The **inbound traffic is free** in most cases. But the **outbound traffic** is not. 
One of the things that I advise you do is go to Microsoft pricing page for bandwidth and read about the scenarios when it comes to how bandwidth is priced because there's quite a few of them, there are different pricing scenarios for moving data across data centers when moving across different regions in different markets or different continents.
It's something I advise you to check if you're designing applications that will have their infrastructures scale globally and you will be moving a lot of data across different Azure regions

![image](https://github.com/user-attachments/assets/3c6606ab-65df-4901-85b9-b65b2d1ede96)


# CHAPTER SUMMARY

![image](https://github.com/user-attachments/assets/66c439e3-117e-40c8-9e23-d0ae100e046b)

