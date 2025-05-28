 <p align="center"><b>What is cloud computing?</b></p>


Cloud computing = delivery of computing services over the internet
Computing services= common IT infrastructure (e.g virtual amchines, storage, databases, and networking)

Cloud services expand the tradiational IT offerings to include things like IoT, ML and AI.

If you need to increase your IT infrastructure rapidly, you don't have to wait to build a new datacenter- you can use the cloud for rapid expand of IT footprint.


Cloud computing lets you choose the power and features you need to run your software. 

The difference is, with Cloud computing, the PC is in a Cloud provider's data center instead of it being physical. With that said, it lets you pay for only the services you use, pus someone else to geth to manage the upkeep of the computer.

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

