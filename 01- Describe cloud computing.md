 <p align="center"><b>WHAT IS CLOUD COMPUTING?</b></p>


Cloud computing = delivery of computing services over the internet

Computing services= common IT infrastructure (e.g virtual amchines, storage, databases, and networking)

Cloud services expand the tradiational IT offerings to include things like IoT, ML and AI.

If you need to increase your IT infrastructure rapidly, you don't have to wait to build a new datacenter- you can use the cloud for rapid expand of IT footprint.


Cloud computing lets you choose the power and features you need to run your software. 

The difference is, with Cloud computing, the PC is in a Cloud provider's data center instead of it being physical. With that said, it lets you pay for only the services you use, plus someone else to gets to manage the upkeep of the computer.

**Each Cloud provider have their own selection of services to choose from, but the basic services provided by all Cloud providers are compute power and storage.**

**Compute power** is how much processing your computer can do. Like when buying a home computer, you may choose computer with 8GbB of RAM and the latest processor to run the software you need currently but as the load on the computer grows, the system slows down. With Cloud computing you can add and remove computer power as you need it. This saves on cost sinc eyou only pay for the resources you use. 

**Storage** is the volume of data you can store on your computer. A traditional computer has limited hard drive space. Over time, you may have to run out and buy another hard drive to store more data. With Cloud computing, you can request more storage as you need it.


Cloud providers manage the upkeep of the computer, they will make sure that there are backups, that the operating system is up to date, as well as making sure that everything is up and running 24 hours a day. 

As business grows and computing needs change, you can quickly bring on new computing resources in a cost effective way. 










<p align="center"><b>DESCRIBE THE SHARED RESPONSIBILITY MODEL</b></p>


  In a traditional datacenter, it is the IT department reposnible for maintaining and ensuring that the infrastructure and software needed to keep datacenter are up and running. It also includes makig sure that securities are updated such as systems patches are applied and on the correct version.

But with **shared responsibility** model, these gets split between cloud provider and the consumer:
  > Physical security, power, cooling, network connectivity = responsibility of the cloud provider


  > Data and information store in the cloud, access security (meaning giving access to those who need it) = responsibility of the consumer




**There are instances where responsibiltiy depends on the situation.**
Examples:
1. For cloud SQL Database, the cloud provider would be responsible for maintaining the actual database. But consumer is still responsible for the data that gets ingested into the database. 
2. If a virutal machine is delployed and installed an SQL database, the consumer is responsible for database patches and updates, as well as maintaining the data and information stored in the database.


The diagram below highlights how the Shared Responsibility Model, this shows us who is responsible for what, depending on the cloud service type.


| Responsibility                              | SaaS       | PaaS       | IaaS       | On-prem   |
|----------------------------------------------|:----------:|:----------:|:----------:|:---------:|
| **Responsibility always retained by customer** |||||
| Information and data                         | ✅         | ✅         | ✅         | ✅        |
| Devices (Mobile and PCs)                     | ✅         | ✅         | ✅         | ✅        |
| Accounts and identities                      | ✅         | ✅         | ✅         | ✅        |
| **Responsibility varies by type**            |||||
| Identity and directory infrastructure        | 🔄         | 🔄         | ✅         | ✅        |
| Applications                                | 🔄         | ✅         | ✅         | ✅        |
| Network controls                            | 🔄         | 🔄         | ✅         | ✅        |
| Operating system                            | 🔄         | 🔄         | ✅         | ✅        |
| **Responsibility transfers to cloud provider** |||||
| Physical hosts                              | ☁️         | ☁️         | ☁️         | ✅        |
| Physical network                            | ☁️         | ☁️         | ☁️         | ✅        |
| Physical datacenter                         | ☁️         | ☁️         | ☁️         | ✅        |

Legend:

✅ — Customer

☁️ — Cloud provider (Microsoft)

🔄 — Shared responsibility












<p align="center"><b>DEFINE CLOUD MODELS</b></p>


Three main cloud models are: **private, public,** and **hybrid**

**Private Cloud**
- A cloud that is used by a single entity.
- This provides much greater control for the company and its IT department.
- Maybe hosted from your on site datacenter, may also be hosted in a dedicated datacenter offsite. Potentially, eveny by a 3rd party that has dedicated that datacenter to your company.
- Cons: it comes with greater cost



**Public Cloud**
- It is built, controlled, and maintained by a third-party cloud provider



**Hybrid Cloud**
- As name says, hybrid of both public and private clouds in an inter-connected environment
- Can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources
- It can provide an extra layer of security
- User can flexibly choose which services to keep in public cloud and which to deploy to their private cloud infrastructure

  

| Public Cloud                                      | Private Cloud                                           | Hybrid Cloud                               |
|---------------------------------------------------|--------------------------------------------------------|--------------------------------------------|
| No capital expenditures to scale up               | Organizations have complete control over resources and security | Provides the most flexibility             |
| Applications can be quickly provisioned and deprovisioned | Data is not collocated with other organizations’ data  | Organizations determine where to run their applications |
| Organizations pay only for what they use          | Hardware must be purchased for startup and maintenance | Organizations control security, compliance, or legal requirements |
| Organizations don’t have complete control over resources and security | Organizations are responsible for hardware maintenance and updates |                                            |


**Multi-cloud**
- Increasinlgy likely scenario is a multi-cloud scenario where multiple public cloud providers are used. This is likely when different features from different cloud providers are used.


**Azure Arc**
- a set of technologies that helps manage cloud environment whether it is a public cloud solely on Azure, a private cloud in your datacenter, a hybrid configuration, or even a multi-cloud environment running on multiple cloud providers at once.



Describe the consumption-based model

**Azure VMware Solution**
- This is helpful when there is an established with VMware a private cloud environment but want to migrate to a public or hybrid cloud. Azure VMware Solution lets you run your VMware workloads in Azure with seamless integration and scalability.




<p align="center"><b>DESCRIBE THE CONSUMPTION-BASED MODEL</b></p>

Two types of expenses to consider when comparing IT infrastructure models:
- Capital expenditure (CapEX) = One time, up-front exenditure to purchase or secure tangible resources
- Operational Expenditure (OpEx) = Spending money on services or products over time

**Cloud Computing** falls under **OpEx** since it operates on a consumption-based model. We pay for the IT resources we use in Cloud computing. If no IT resources are used this month, you will not pay for any IT resources.

**Benefits of consumption-based model:**

- No upfront costs
- No need to purchase and manage costly infrastructure that might not be used to its fullest potential
- The ability to pay for more resources when in demand
- The ability to stop paying for more resources when no longer needed


<p align="center"><b>COMPARE CLOUD PRICING MODELS</b></p>

Cloud computing delivers computing services over the internet by using the **"pay-as-you-go"** pricing model. As mentioned previously, you pay only for the cloud services you use and these helps you:

- Plan and manage operating costs
- Run your infrastructure more efficiently
- Scale as your business needs change

  To put it simply, with cloud computing, you are renting compute power and storage from someone else's datacenter. It is as though you are using resources in your own datacenter except tgat when you are done using cloud resoruces, you give them back and you get billed only for what you use.


- More resources:

- Run VMware resources on Azure VMware Solution
https://learn.microsoft.com/en-us/training/modules/intro-azure-vmware-solution/1-introduction


- Introduction to Azure hybrid cloud services
https://learn.microsoft.com/en-us/training/modules/intro-to-azure-hybrid-services/


- Shared responsibility in the cloud
https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility


  
