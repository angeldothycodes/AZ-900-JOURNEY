![Screenshot 2025-06-03 080044](https://github.com/user-attachments/assets/a2d1ef80-8ef9-459d-8cde-38cab63ef47a)

Cloud computing is a delivery model for services. Services like storage services as whenever you're storing your unstructured or structured data in files and databases while delivers ypu thousands of servcies to do so.

You pretty much can choose any technology that is popular in the market and you will be able to use it with an Azure environment. In this case, storage doesn't only mean storing data but also all the services and tools that allow you to migrate your data to the cloud.


Once data is in the cloud, **computer resources** will be needed like a Windows virtual amchines, maybe a Linux ones, web containers or any of the hundreds of services available in the cloud because cloud is about creating applications whenever those are web, AI, machine learning, reporting, any kind of applications out there. Additionally, once you have your components, you need to be able to somehow connect them to each other securely. 

Cloud delivers you with said functionalities to create secure networking between those components but also your company. And because your entire platfrom is managed in the cloud, cloud also needs to delvier **analytic capabilities** so you can review your performance and telemetry data for your services. 

There are many list of services clouds can offer but these four are the main ones and that are tested by the exam.


All of those ervices are delivered over the internet and this is bascially what cloud is.



![image](https://github.com/user-attachments/assets/44c93211-98b1-4724-a7eb-067b0650a0e9)


**Delivering services like this doesn't make a cloud computing yet**

Computing needs also fulfill certain characteristics. First, scalability. Imaging there is a resource like a web app, vm, database, etc.
And it needs to be scale up by increasing size. Increasing size means increasing resources like CPU, memory, or maybe faster storage. In this case, we are moving along the vertical line. That's why this is called **vertical scaling**. Increasing the size of the resource is called scaling up. If you decrease the size, decrease the power of the machine, this is called scaling it down.
Besides changing the size of the resource, changing the power of that resource, you can also scale by adding more resources to your environment. 
Increasing the amount of the resources themselves, in this case we are moving along the horizontal line that's why this is called **horizontal scaling**.
Increasing the amount of your resources, this is called **scaling out**. If you decrease the amount of resources, this is called **scaling in**


![image](https://github.com/user-attachments/assets/b5602c4c-1321-47f6-b8e6-78b86525d25b)


![image](https://github.com/user-attachments/assets/c0782c3b-b8b7-4b22-8858-57c9e7f64419)



<h3 align="center">Elasticity</h3>

Best way to explain elasticity is to show to user workload off in the typical application during the day where the user workload changes as the day progresses. If you design system like this, you need to assign the specific amount of resources to be able to handle the workload. Properly designed system will be able to allocate and deallocate resources whenever needed. If this process is done automatically, this is **automatic scaling**. An **automatic scaling** is basically what **elasticity** is.

**To summarize, elasticity is the ability of the system to scale dynamically.**




<h3 align="center">Agility</h3>

In the cloud, there are two ways to provision resources: manually via portal or automated ways using APIs and scripting. Regardless of what choice you make, there is time between the request is submitted and the response that the request has been fulfilled.

Major difference between cloud and on-premises is that requesting resources in on-premises usually takes days, weeks, or even months. In cloud, once you request the resource, you will likely get it within seconds or minutes. For very big services, this might take few hours but still this is a major difference between the on-premise environments. In this case, when we say **agility**, it is the ability to react quickly and in the cloud this means being able to allocate and deallocate your resources in very short time. 




<h3 align="center">Fault Tolerance</h3>

As a user, you purchase services from the cloud whenever that's web application, Virtual machine, or SQL but regardless of the service you choose or interface that you use that service with, all those services need to run on some sort of servers in a datacenters. Storing their data on disk arise whenever there's any service or component failures on those servers were out on to be moved to another and same goes for disks arrays. Your data is ultimately stored on multiple discs and multiple disk arrays. To ensure no data is lost, both tolerance in this case talks about the ability of the system to remain up and running during component and service failures. Localized failures will not interrupt your service most of the time. In the cloud, all of the services have built-in fault tolerance, that means if you use cloud services, you will not notice those localized failures affecting your system at all. 


![image](https://github.com/user-attachments/assets/99d3e507-e563-4146-a2e6-be4233aee2bc)
![image](https://github.com/user-attachments/assets/06f6b992-8eb6-4682-9467-3f87528153d9)


Besides those localized failures, an event of much greater scale might happen and event like this is called disaster. Disaster is a serious disruption of services caused by natural or human-induced causes. What we need t do is set up disaster recovery. Disaster Recovery simply means creating two copies of the same application into Azure regions and setting up replication between them so that there is two identical copis of data/ application. In front of those application, a simple DNS routing is need to be setup so that users are automatically redirected to the working version of your application. If any service failes, they will automatically get redirected to replicated version of application. 

![image](https://github.com/user-attachments/assets/02cbac29-c44e-43e5-b53b-1e961c94f03a)




<h3 align="center">High Availability</h3>

High Availability is a simple metric that measures how much uptime of the system so the
