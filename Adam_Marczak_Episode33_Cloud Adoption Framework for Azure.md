![image](https://github.com/user-attachments/assets/cebb4020-2614-4a96-ac64-de3838b5ca37)


# Cloud Adoption Framework

As part of the exam and this episode, you should be able to understand and describe the key elements of cloud adoption framework and how does it help with the adoption process itself. 

Before we move to the framework itself, let's start with **what cloud adoption is**

**Cloud Adoption** is simply a strategic move by your organization, your company in order to leverage cloud in their current business. This is done simply because cloud has a lot of things to offer, to accelerate your business and allow you to innovate and build soutions faster therefore, provide more value to your customers. 

![image](https://github.com/user-attachments/assets/074abd0d-c185-4b60-a29a-c32a8a46c40e)


**Cloud adoption framework** is a set of tools, best practices, guidelines, and documentation created by Microsoft to help companies with the journey.

![image](https://github.com/user-attachments/assets/db9116e4-821f-4081-bebc-ac66f9a547ec)


**Cloud adoption framework** is divided into stages:

1. The first stage we'll look at today is called **Strategy**. 
**Strategy** is simply building organizational alignment for moving to the cloud, to begin cloud adoption.

**a.** The first step step in the strategy is called **motivations**. During this step, you want to answer the question **why move?** As such, you want to meet with your key stakeholders and executives in your company to document what are the motivations behind the cloud adoption. To do that you need to understand what are your motivation triggers. The most common motivation triggers are either migration triggers- moving your current infrastructure to the cloud so that you can some cost savings, you can reduce the complexity of your current infrastructure, maybe you want to optimize your current operations or increase business agility by having more flexible approach to managing infrastructure.
Another motivation trigger is called **innovation**. In this category, you want to leverage the cloud and its features to provide some improvements to your company. For example, maybe reaching a global scale or improving customer experience. Maybe you want to disrupt new markets or create new products or services. All of those are easier to do if you start using the cloud with all of its features.

![image](https://github.com/user-attachments/assets/05074db0-47a7-4569-95fb-c591bd3139b5)

**b.** Once we understand why move, the next thing you need to do is so-called **business outcomes**. In the **business outcomes**, you want to answer the questions **what to measure** so what would be your criteria of success that would support your move to the cloud. This measure has to be a defined, concise observable outcome for your company. Typical things might include an increase in revenue and profit or cost reduction or maybe something more business oriented like having a global access and reaching new markets but it is important that this measure can be calculated and can be observed s that you can define it and track it. In this process, you will want to meet with your business leaders from the finance, IT infrastructure, and application groups. 

![image](https://github.com/user-attachments/assets/adf184b5-922d-4cfc-b643-7419ef4ebea2)

**c.** When we know what to measure and why do we move to the cloud, next thing is business justification. During this step, we need to understand what is my return of investment because your company is there to make money and it is important to track it and this is what this step is all about. As part of the business justification, you will want to develop a business case that will create a financial model that supports both motivations and the outcomes. This business justification will use the input from the two previous steps. There are many tools provided by Microsoft that supports you in the process of building this financial model. For example, a persone like a CFO (chief financial officer) in your company might want to use **Azure TCO** which stands for **Total Cost of Ownership calculator** to calculate the cost of your current on-premise infrastructure. With Azure pricing calculator, you can estimate the monthly cost of Azure Infrastructure. 
Once you start deploying things to Azure, **Azure Cost Management** will give you a full visibility on the existing resources and their cost. 

![image](https://github.com/user-attachments/assets/af9fdc90-d9f1-4f62-83b9-8716d55dae17)

**d.** Lastly, we want to decide on the **First Project**. This first project will help you align your motivations and technical efforts. To choose the right first project, you need to follow **two criterias**, first criteria is so-called **business criteria**. In here, you want to find a project that is first of all currently operating. The project that is constantly working your company na dhas dedicated owner, but this is very important that this owner and this application has a strong motivation to move to the cloud because it sees its benefits. This is important because the engagement of the owner will be very important cross every single step of the process. Additionally, there are **technical criteria**. You want to find a project that has minimum amount of dependencies and assets. This is because if you choose a project that is too big, it will take you too long to validate your strategy.

![image](https://github.com/user-attachments/assets/46f95a67-3247-4d0b-a1c5-7e573561f6f8)

**In summary, our first stage, **strategy** is about defining business justification and the outcomes. Once the stage is completed, we move the **planning phase**.

In the **planning phase** there are again few steps that we need to follow. 

**a.** The first step is **Digital Estate**. This is so-called **investory of assets**. You want to review what you currently have in your company and what you should do with it. And that decision, that rationalization is decided bases on the **five R's** of rationalization rule. For each digital asset that you will find in your company, you want to assign one R. 

**1.** First, we have **rehost**. **Rehost** means that we take existing application and we move it to the cloud without any changes. This typically means move existing applications into infrastructure as a service (IaaS)- deploy into virtual machine or a container. 

**2.** Another **R** is **refractor**. You want to make a small changes to your existing application codebase in order to fit it into existing Platform as a Service (PaaS) offerings in Azure. For example, if you have a web application running on a virtual machine and it uses SQL server, maybe with a little bit changes in your code, you can fit it to Azure App Service and Azure SQL to take advantage of the Platform as a Service (PaaS) offering in Azure.

**3.** Another option is called **rearchitect**. For the **rearchitect**, you will need to make complex changes to your codebase. This is used to introduce new services in your application. For example, you might see that a key vault is very good service in Azure and you want to introduce it in your application therefore you might want to rearchitect existing ones to take advantage of those security services in Azure. Another reason for rearchitecture is when your application strongly depends on the physical infrastructure in your company so it is incompatible with the cloud. In short, you use rearchitect to implement new features or fix incompatible applications. 

**4.** Another one is **rebuild**. For this rationale, we create applications from scratch. This could be also called New. We look at existing application, we see that effort of introducing this in the cloud is too big or maybe the code is too old and we decide to rebuild this from scratch to take full advantage of what cloud has to offer 

**5.** The last one is called **replace**. In **replace** you want to look at every single application that you have and see what cloud has to offer already. Maybe not only Azure but Office365 has a lot of Software as a Service offerings. Maybe there is offering that completely replaces the functionality that your current application provides. In which case you might want to drop the current application and take the Software as a Service offering. Basically, in your company go though every project that you have

