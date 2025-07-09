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

One thing to note is that resources that are only organizational resources and logical resources like **Resource groups** are free because they are not servers, they are logical objects in Azure. Those do not have any kind of cost associated.

What you should remember from this slide is that every resource type have a small metric that is tracking its usage and this will be your key factor that will affect the final cost of your Azure environment. Therefore you should always spend time to think what kind of use case do you have. What kind of application are you building and which are the right resoruce types for you.

![image](https://github.com/user-attachments/assets/b04d67dd-2b1b-42b3-b62e-8cb33724b928)
