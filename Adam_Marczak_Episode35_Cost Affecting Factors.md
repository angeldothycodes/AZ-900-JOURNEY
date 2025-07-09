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

Besides that you can contact Microsoft representative and buy an enterprise agreement. This is agreement between your company and Microsoft. This is a contract that you sign. Lastly, you can buy Azure from a partner of Microsoft so-called **Cloud Solution Providers**. This model in short is called CSP. So depending on which Azure offer type do you have, it will affect two things. One of them is **usage rate**, simply the cost of your **Azure services** and the billing cycle but the usage rates are changing because when you are purchasing Azure from an enterprise agreement or through CSP, you can negotiate the prices. If you negotiate any discounts, this discount will be applied
