![image](https://github.com/user-attachments/assets/06c7c4cb-2d6e-4d96-aa32-f06e0fa459b5)


## DATA CENTER
> If you purchase services in Azure, whenever this is SQL database, web hosting, virtual machine, or one of many services within Azure - all those services run on a physical infrastructure underneath on some sort of servers. A physical facility that host those servers is a data center. It is used to host a group of network servers. A typical data center has its own power, cooling, and networking infrastructure.
>
> So data centers are building blocks of global Azure infrastructure
>
> ![image](https://github.com/user-attachments/assets/3b75260d-4e6f-4919-b590-ae19027b9ba3)
>
> A group of datacenters that are connected with each other with high throughput internet connectivity are called regions and Microsoft has many regions across the globe of different sizes, they can be as small as single data center or they can contain multiple ones
> but what is most important is that they are globally distributed. For instance, in united States , you have one in East US and one in West US. In Ireland, there's a North Europe region and in Singapore, we have Southeast asia region. There's also one in Japan  called Japan east but there's plenty more regions available. If you start putting a dot for every region available within Azure, we would get over 50 dots on that map. Being able to choose from whatever location we want on the planet to be as close to our clients as possible. This is important decision for every Azure developer and architect because the closer you are to your cleints, the lower the latency between the servers and your clients.

![image](https://github.com/user-attachments/assets/7bf2094a-01cd-496a-b16d-eb82619a7768)

When it comes to region, there are few things you need to understand. First of all, region is simply a geographical area on the planet that consists one but usually more data centers but they need to be connected with low latency network. We are talking here about 2 milliseconds latency between the data centers.
Additionally, this is the location for your services. Location is a word that will come up very often when you work with Azure. Whenever you purchase any Azure ervice, a location will always be mandatory field that you will need to fill and it simply means to which physical servers on the planet, which region on the planet should I deploy that service to.
There are also few very important things to remember, first of all, some of these services are not available in all the regions. You shoud always check which region has the services that you need to build your application.

There are also some services that are called global services. Those services don't have any specific region and specific location assigned- things like traffic manager for DNS routing or Azure AD but there are a few other examples  here. 

Additionally, Azure is globally available with over 50 regions available. New regions are being announced and built pretty much everyday. So in future, there might be more than that and lastly, there are some special regions like government regions for government regulations and partner regions like China regions where Microsoft is providing the services but it doesn't really manage the services themselves 


![image](https://github.com/user-attachments/assets/9de55eab-f56d-45f9-9bdd-1214b4bb3207)



## AVAILABILITY ZONE
