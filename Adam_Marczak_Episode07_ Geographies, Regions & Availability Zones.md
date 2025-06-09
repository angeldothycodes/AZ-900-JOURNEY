![image](https://github.com/user-attachments/assets/06c7c4cb-2d6e-4d96-aa32-f06e0fa459b5)


## DATA CENTER
> If you purchase services in Azure, whenever this is SQL database, web hosting, virtual machine, or one of many services within Azure - all those services run on a physical infrastructure underneath on some sort of servers. A physical facility that host those servers is a data center. It is used to host a group of network servers. A typical data center has its own power, cooling, and networking infrastructure.
>
> So data centers are building blocks of global Azure infrastructure

![image](https://github.com/user-attachments/assets/3b75260d-4e6f-4919-b590-ae19027b9ba3)

> A group of datacenters that are connected with each other with high throughput internet connectivity are called regions and Microsoft has many regions across the globe of different sizes, they can be as small as single data center or they can contain multiple ones but what is most important is that they are globally distributed.

![image](https://github.com/user-attachments/assets/ad59caf8-f491-425b-89b6-ab6cf94cee8d)

For instance, in united States , you have one in East US and one in West US. In Ireland, there's a North Europe region and in Singapore, we have Southeast asia region. There's also one in Japan  called Japan east but there's plenty more regions available. If you start putting a dot for every region available within Azure, we would get over 50 dots on that map. Being able to choose from whatever location we want on the planet to be as close to our clients as possible. This is important decision for every Azure developer and architect because the closer you are to your cleints, the lower the latency between the servers and your clients.

![image](https://github.com/user-attachments/assets/7bf2094a-01cd-496a-b16d-eb82619a7768)

When it comes to region, there are few things you need to understand. First of all, region is simply a geographical area on the planet that consists one but usually more data centers but they need to be connected with low latency network. We are talking here about 2 milliseconds latency between the data centers.
Additionally, this is the location for your services. Location is a word that will come up very often when you work with Azure. Whenever you purchase any Azure ervice, a location will always be mandatory field that you will need to fill and it simply means to which physical servers on the planet, which region on the planet should I deploy that service to.
There are also few very important things to remember, first of all, some of these services are not available in all the regions. You shoud always check which region has the services that you need to build your application.

There are also some services that are called global services. Those services don't have any specific region and specific location assigned- things like traffic manager for DNS routing or Azure AD but there are a few other examples  here. 

Additionally, Azure is globally available with over 50 regions available. New regions are being announced and built pretty much everyday. So in future, there might be more than that and lastly, there are some special regions like government regions for government regulations and partner regions like China regions where Microsoft is providing the services but it doesn't really manage the services themselves 


![image](https://github.com/user-attachments/assets/9de55eab-f56d-45f9-9bdd-1214b4bb3207)



## AVAILABILITY ZONE

![image](https://github.com/user-attachments/assets/c638945b-cfb9-4bf1-a5a2-b3a778c97643)


This is a regional feature where each data center gets a number that represents a grouping of physically separate facilities 
Simply said availability zones are designed to protect from data center failures because each availability zone has its own power cooling and network infrastructure whenever there's a failure in a single datacenter, others will continue working. if you think about it this is how datacenter operates normally. 

**How does availability zones help here?**
By introducing this feature, Microsoft also created services and features within services that can take advantge of this information. Those services are split into two categories. The first ones is **zonal services**. With zonal services, you can choose to which availabilityzones are you doing the deployment to. In case of virtual machines, now you have a choice. You can create two virtual machines for highly avilable environment and specy that the first virtual machine goes to availability zones # 1, and second one goes to availability zone #2 or 3. This way, you ensure that if there's a datacenter-level failure, at least one of your VM will continue working. In the calssical scenario, without availability zones, it is possible that your VM even in a big region could be deployed in the same data center or even to the same physical server that is why **availability zone** allow you to create those highly available applications

The secodn type of the service is **zone-redundant service**. Those services like SQL database, storage accounts, allow you to take advantage of multiple availability zones out  of the box. With a simple check of an option, your services will automatically replicate data across multiple availability zones and will work in a redundant way. So if there's a data center-level failure, you wouldn't even notie it in your application. 



**Few things that you should note here**

![image](https://github.com/user-attachments/assets/d8fb72c2-5cb9-4346-b751-24824083f22c)

- First of all, not all regions support availability zones. About seven regions right now support it with more coming in the future.
- Second, if the region supports it, there's at least three or more zones within that region. That means there's at least three data centers required
- Lastly, availability zone is built from one or more data centers. It's not necessarily a single data center


If we look at our map, some Azure regions will have logical groupings over their data centers makig them zone-enable region. 

![image](https://github.com/user-attachments/assets/b7eddf52-91f3-4348-bc2f-a657e627cdb2)

**What happens if there's a region-level failure, if entire region goes down?**
Then it doesn't matter if you use availability zones. For that reason, Microsoft created **region pairs**. Each region has a **region pair**. Paired regions are at least 300 miles away from each other to ensure that there's enough distance to cover the natural-level disaters (e.g. floods, storms, earthquakes, etc.)

This way Microsoft ensures that if one region goes down, the second region that is paired with that region will be up and gives you a set of features to allow you to replicate your data, application, across multiple regions

![image](https://github.com/user-attachments/assets/7d6533ff-05e3-4b8c-b0c2-bd261bff5bbc)



## Region Pairs
- Each region is paired with exactly one region
- Each region pair is sttaic. You cannot choose region are you pairing to, Just check the documentation to which region you see your region currently.
- Each region also resides within the same geography (with an exception of a single Brazil south which is replicating to US)
- Each region pair has physical isolation of at least 300 miles distance from each other - to ensure that large-scale natural disaster will not take two regions down at the same time
- One of the cool features of region pairs is that some services will provide a platform-level replication. Again, with a simple check of an option, you will automatically replicate your data and your services across multiple regions. Therefore, protecting yourself from region level failures
- Additional benefit of region pairs is that Microsoft is palnning updates across pairs. Therefore, if you will replicate to another pair, Microsoft is making sure that the plan updates, plan rollout of the services don't happen to the same paired regions at the same time. Therefore, it will rollout all the updates and all the necessary things to the first regions, if everything is working correctly, the updates wil be rolled out to the spared region making sure that even the platform updates will not impact your application. therefore, it is preferred option for you to replicate to a paired region.
- If you are planning for disaster recovery scenarios, you can ensure data resiliency is maintained for your applications

![image](https://github.com/user-attachments/assets/9be6a07c-30dd-4ecf-a0aa-2e9abfabdd79)


![image](https://github.com/user-attachments/assets/07f45bad-f22d-4a90-b98e-5a91828f83bc)

