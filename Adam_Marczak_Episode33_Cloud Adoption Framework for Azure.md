![image](https://github.com/user-attachments/assets/cebb4020-2614-4a96-ac64-de3838b5ca37)


# Cloud Adoption Framework

As part of the exam and this episode, you should be able to understand and describe the key elements of cloud adoption framework and how does it help with the adoption process itself. 

Before we move to the framework itself, let's start with **what cloud adoption is**

**Cloud Adoption** is simply a strategic move by your organization, your company in order to leverage cloud in their current business. This is done simply because cloud has a lot of things to offer, to accelerate your business and allow you to innovate and build soutions faster therefore, provide more value to your customers. 

![image](https://github.com/user-attachments/assets/074abd0d-c185-4b60-a29a-c32a8a46c40e)


**Cloud adoption framework** is a set of tools, best practices, guidelines, and documentation created by Microsoft to help companies with the journey.

![image](https://github.com/user-attachments/assets/db9116e4-821f-4081-bebc-ac66f9a547ec)


**Cloud adoption framework** is divided into stages:

# STRATEGY

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

**In summary, our first stage, **strategy** is about defining business justification and the outcomes. Once the stage is completed, we move the **planning phase**.**

# PLANNING

In the **planning phase** there are again few steps that we need to follow. 

**A.** The first step is **Digital Estate**. This is so-called **investory of assets**. You want to review what you currently have in your company and what you should do with it. And that decision, that rationalization is decided bases on the **five R's** of rationalization rule. For each digital asset that you will find in your company, you want to assign one R. 

**1.** First, we have **rehost**. **Rehost** means that we take existing application and we move it to the cloud without any changes. This typically means move existing applications into infrastructure as a service (IaaS)- deploy into virtual machine or a container. 

**2.** Another **R** is **refractor**. You want to make a small changes to your existing application codebase in order to fit it into existing Platform as a Service (PaaS) offerings in Azure. For example, if you have a web application running on a virtual machine and it uses SQL server, maybe with a little bit changes in your code, you can fit it to Azure App Service and Azure SQL to take advantage of the Platform as a Service (PaaS) offering in Azure.

**3.** Another option is called **rearchitect**. For the **rearchitect**, you will need to make complex changes to your codebase. This is used to introduce new services in your application. For example, you might see that a key vault is very good service in Azure and you want to introduce it in your application therefore you might want to rearchitect existing ones to take advantage of those security services in Azure. Another reason for rearchitecture is when your application strongly depends on the physical infrastructure in your company so it is incompatible with the cloud. In short, you use rearchitect to implement new features or fix incompatible applications. 

**4.** Another one is **rebuild**. For this rationale, we create applications from scratch. This could be also called New. We look at existing application, we see that effort of introducing this in the cloud is too big or maybe the code is too old and we decide to rebuild this from scratch to take full advantage of what cloud has to offer 

**5.** The last one is called **replace**. In **replace** you want to look at every single application that you have and see what cloud has to offer already. Maybe not only Azure but Office365 has a lot of Software as a Service offerings. Maybe there is offering that completely replaces the functionality that your current application provides. In which case you might want to drop the current application and take the Software as a Service offering. Basically, in your company go though every project that you have, assign one of those **Rs** for every project that you can and then create a plan out of this.


**B.**

Next step is **Initial Organization Alignment**. During this, when the plan is being established, you want to meet with the key stakeholders in your organization to make sure that everyone is aligned and every key person supports this adoption plan. During this step, the alignment of people who will make this plan a reality is very important. It is also a step where you map your people to the capabilities so you know who should be engaged when. 

**C.**

Once your organization is aligned, you will create **Skills Readiness Plan**. During this stage, you want to review your current skill sets in your company and create a plan that will address the gaps because in the cloud, you will need to have a lot of new skills in your company across different teams and different people and this plan will take care of that.

**D.**

Once you do all those things, simply put it into so-called **Cloud Adoption Plan**. This plan will be used to manage the change across your digital estate, skills, and the organization and the processes.

### SUMMARY

In the planning stage, we want to create actionable plan for our cloud adoption. From there, we move to the next stage called **ready**.

# READY

Readiness stage is all about preparing your first Azure environment. To do that, you start with **Azure Setup Guide**. You read Azure documentation on how the initial environment should look like. You want to become familiar with the tools and approaches that will help you create this first Azure Environment. Also, at this stage, you will want to choose which type of Azure subscription should you use and which is best for yur company. Once you have everything prepared, you start creating your first Azure environment. This is so-called **Azure Landing Zone**, this will be your first Azure environment. It will be completely created out of Microsoft guidelines and it will allow you to setup a codebase for future improvements. An advice here is to use infrastructure as a code approach so that everything can be later changed, expanded, updated but everything will be consistent and very easy to redeploy if needed.

Once the landing zone is created, you want to extend it even further (**Extend Landing Zone**) to match your organization needs and allow for the smooth cloud transition. One important thing is this will be shown across this entire process and a lot of places in cloud adoption framework is as you go through those stages **always check the best practices**. You just want to be sure that this initial landing zone and the expansion goes according to the best practices because later on it's very hard to change things if you will create bad platform architecture.

![image](https://github.com/user-attachments/assets/e1cd34a0-8c9b-4130-aef1-b526a6ed8294)





# ADOPT

To summarize the ready stage, we want to prepare Azure environment since we have the plan to adopt the cloud. Our next step is **Adopt**. Because all our previous stages were preparing us to move to the cloud. **Adopt** is where we start doing that. In the adaoption, we again, have few steps but adoption splits into two separate streams. One is called **migrate**. When we are talking about motivations, one of the most common motivation triggers was migrations and this is why adoption is split into migrations and innovations. The first step that you want to do in this stage is do your first migration.
During this step, you want to migrate your first project to the cloud. This is so that you can read all the guides that Microsoft prepare for the migration paths. You want to familiarize yourself with the native tools and approaches in Azure that will help you to do that migration. But the important part here is not only the migration but also the learning curve. Because after the first migration you need to familiarize yourself with migration scenarios. When moving to the cloud, you will see that there's plenty of different scenarios, different workload that needs to be migrated. 

For example, migrating virtual machines is completely different from migrating data services or maybe web applications. Microsoft has plenty guides that are available for you to use during this process. You need to familiarize  yourself with those and prepare migrations scenarios for your own company. Just like with the previous step, remember to also check **Best Practices** because migrating is one thing but also setting everything up is another so make sure that your architectural decision will follow the best practices
