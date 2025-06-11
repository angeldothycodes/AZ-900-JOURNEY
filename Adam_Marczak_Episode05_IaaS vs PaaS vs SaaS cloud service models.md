

Small exercise: let's imagine we are a startup company and we want to host our own application and build entire infrastructure for that reason. First thing we will need to do that is to purchase some servers. All the hardware that will actually run the applications themselves. Obviously, our servers needs to be able to connect to the Internet, therefore, we will need to provide all the networking infrastructure including the Internet connectivity itself. Because every server needs a storage, you will need to additionally provide a storage infrastructure. And those are hard drives or SSD, some RAID arrays, etc.


Once this is in place, you have all the hardware needed in order to run the server. In order to ensure the best utilization of the hardware that you have, you will want to run some virtualization to run mutiple virtual machine on a single hardware piece to host multiple applications but still maintaining the separations of the environemnts. All those virtual machines will needs an operating systems (Windows, Linux, or any other OS on the market), a middleware which typically means all the software additions that you need in order to run the system and the application itself. A typical application will additionally need a runtime- if this is a web application this could be IIS web container, if it's a container application then maybe Docker. But runtime is additional layer that you will need to maintain yourself. Once those layers are in place, we are now finally ready to host our application and application data on that system. 



| Layer                | Components                           |
|----------------------|--------------------------------------|
| Storage              | HDD, SSD                             |
| Networking           | Routers/Switches, Internet           |
| Servers              | Memory, Motherboard, CPU             |
| Virtualization       | VM (Virtual Machines)                |
| Operating System     | Windows, Linux                       |
| Middleware           | Software                             |
| Runtime              | IIS, Docker                          |
| Applications Data    | Data, Apps                           |



![image](https://github.com/user-attachments/assets/b60e7f45-413d-4e78-bcd5-d053d995ac79)



![image](https://github.com/user-attachments/assets/552fe9b5-00f3-474f-83a3-23e207257ebb)



**WHO WILL MANAGE WHAT?**

**On-premises** 
> You manage all of those layers
> Clear ownership is on you. You manage all the infrastructure, platform, and the software.


![image](https://github.com/user-attachments/assets/fbf1123b-527c-4fec-9b30-ab7005fff0bb)



If you decide to outsource the infrastructure, purchase the infrastructure from the cloud provider, to let Microsoft manage the infrastructure while you manage the platform and software, this is so called **Infrastructure as a Service**. In this case Microsoft will manage all the networking, hardware, and the virtualization itself while you manage the platform and the software part.

![image](https://github.com/user-attachments/assets/16bbd2f9-b515-4dfc-acee-9346c3e78673)


The list of services used in Azure to implement **IaaS** is quit long but typically, you will see things like virtual machine, virtual networks, managed disks or one of many services that you can use for this purpose. In general, the rule of thumb is if someone says that they have IaaS solution, that means they have a lot of virtual machines and probably this is the skills they are looking for. 

If you're designing for the cloud, you most likely will go one level up so you will allow Microsoft to manage the platform and the infrastructure part while you just build your own applications. In that case, we are talking about **Platform as a Service**. In this model, cloud provider will manage the infrastructure and the platform. Besides the hardware, Microsoft will manage the operating system, all the security patches, all the middlewre, and the runtime to host your application. You will only need to build and manage your own applications. Typically this model is used whenever you are developing cloud applications. This could be a state-of-the-art web applications, AI, machine learning, business analytic solutions. If you're building applications, you are most likely using **PaaS** solutions. In this case, we can talk about SQL for relational databases, app service for web hosting, logic apps for enterprise integrations, functions apps for serverless are one of the dozens or even hundres of other services allowing you to take advantage of cloud in a platform as a service model.


![image](https://github.com/user-attachments/assets/ed5b6ad1-4073-440a-82b6-3eef10fa9a87)


![image](https://github.com/user-attachments/assets/cca3d2a7-c423-4855-8d0f-4923a5319e21)


If you decide to outsource everything to Microsoft, that means you are using **Software as a Service** model. The ownership of the cloud provider is everything and there's nothing on you. You could think what would be the case of software as a service, usually this means buying-of-the-shell applications. Applications like Outlook, Skype, OneDrive, and all the business applications that you are probably using everyday, This is **Software as a Service** from Microosft manages everything and you just use the applications. 

![image](https://github.com/user-attachments/assets/6b542d00-37c8-4032-a923-a1b7cd57dde9)


Summarizing the differences from those service models but from a little bit different angle. If you let cloud provider manage the physical datacenter buidlings, networking, security, servers, and the storage, we are talking about **Infrastructure as a Service**. If that cloud provider additionally manages the operating system and the development tools, we are talking about the platform as a service. If that cloud provider additionally manages the applications and the data, we are talking about the software as a service.

![image](https://github.com/user-attachments/assets/0ee0040d-606d-4a27-8646-e8714a59aaca)

