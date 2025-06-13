![image](https://github.com/user-attachments/assets/05bb5f44-e34f-4f35-b24d-1469825385d1)![image](https://github.com/user-attachments/assets/a646310f-fc0d-4f36-9b27-95801ffb7147)

![image](https://github.com/user-attachments/assets/78af2a61-8b30-44fa-b5c3-4bcfc1939e32)

## Azure Virtual Network

Imagine you have two resources in Azure, let's say 2 virtual machines. Because Virtual Machines are representation of the physical hardware in the cloud, they also need to be placed in the representation of the physical network infrastructure. That representation in Azure is called Azure Virtual Network. Virtual Networks allow their customers to create, manage, monitor, and secure connectivity between Azure resources but also between Azure resources and their on-premise environments. 

![image](https://github.com/user-attachments/assets/757824b8-f1a9-4bc4-a6f8-fe3d7fdd5c82)

**Virutal Networks** can be segmented into smaller pieces called subnets. There are two main purposes for having subnets. One is to allow customers to manage their IP address allocation in a more efficient manner but also to group related resources together. So that you can apply filters and security rules across multiple resources within the same subnet.
For example, by grouping all the resources, hosting your web applications and only allowing web traffic to go to that subnet.
As a customer, you have a freedom of how you manage subnets and virtual networks. 
If you want, you can group multiple resources within the same subnet. It is you choice how you want to represent your networking infrastructure in the cloud.
There are many reasons why you would want to have virtual networks and many technical limitations forcing you to do that. For example, virtual network can ONLY reside within a single region and spawn resources from that specific region.
So if you will be building multi-region applications, you will end up with multiple virtual networks.
If you will want to connect multiple virtual networks you can do one of two things. You can either use a feature called **vnet peering**. 

![image](https://github.com/user-attachments/assets/63747437-23c8-4e72-9ef0-d6eb0149542e)

**Vnet Peering** allows you to combine virtual networks together and allow them to act as one or you can use **VPN Gateway** to do so while there are benefits and drawbacks of using one or another. It is a little bit too advanced topic for Azure fundamentals. For now, just remember you have two options and those are **vnet peering** and **VPN gateway**

### Summary
Azure virtual network is an emulation of a physical network infrastructure in the cloud. It is designed to allow customers for isolation and segmentation of their network to enable communication filtering and routing between Azure and On-premise resources. Remember that virtual networks are scoped to a single region, so in multi-region architecture you will have multiple virtual networks which you can connect to each other using either vnet peering or VPN gateway. When it comes to segmentation part, you can achieve that using subnets. Subnets allow customers to divide virtual networks so that they can better and effectively manage their IP addresss allocation but also manage network filtering  for something called Network Security Groups or Application Security Groups.

![image](https://github.com/user-attachments/assets/5b2ced57-4f92-45be-8f0e-33867828544c)


## Network Security Groups

Imagine you have two virtual machines within a single virtual network placed in two separate subnets. If you want to control the traffic that comes from the internet to that virtual machine, you can place a **Network Security Group** on that subnet and those security grous will only allow specific traffic to reach that virtual machine. You can also use network security groups to manage the traffic across subnets. It is a tool to manage your networking in secure and efficient manner.

![image](https://github.com/user-attachments/assets/62d44e7d-16cb-4c05-8e24-f4bfbe660d02)


## Virtual Network Gateway

Also called **VPN Gateway**. VPN Gateway allows you to connect to your on-premise environments so you can enable your virtual network to talk to the network within your on-premise environments. This communication is done over the public internet but it is entirely encrypted. Additionally, VPN gateway can be also used to connect virtual networks to each other although this is a less common case, it is still able to do that. Remember touse VPN gateway whenever you need to connect on-premise environment to azure over the public internet. Or if you need to implement cross-regional communications of Azure virtual networks.

![image](https://github.com/user-attachments/assets/8afd71c7-5370-4134-990f-34ffcfcc7307)


## Azure Load Balancer

Load balancing simply means distribution of the trafiic across multiple resources. So if you have two virtual machines, you can create a load balancer in front and evenly distribute the traffic across those two virtual machines. There are many reasons to do that. One of them is scalability because by adding additional instances, scaling out, you can scale to accommodate much larger workloads versus scaling up where you simply add more power to the machine. The second reason is high availability. If those virtual machines would be a premium virtual machines, by default, from Microsoft you will get three nines (99.9) of SLA. That means each virtual machine is guaranteed to run 99.9% of the time but if you put those virtual machines into separate availability zone and put that in front of the load balancer then Microsoft guarantees 4 nine (99.99%) of SLA. In which ase, you increase SLA and availability for your application by 10x. This is because load balancer automatically checks the health of the application components that its connected to. So if one of the virutal mcachiens stop working, it will redirect the traffic to the second one and the chances of both of them not running is significantly lower than with one virtual machine.


![Screenshot 2025-06-13 074004](https://github.com/user-attachments/assets/6effdb2c-2817-4e55-bf91-05768b9ca4c6)


When you build larger solutions, you will also separate your application components into tiers. For instance, by separating all the components that are handling web traffic into web tier, and possibly second tier handling all the data management for the application having its own balancer to manage internal traffic. In this case, you would have two load balancers. One with public IP, allowing for public internet traffic to come in - it will be called **public load balancer**. And one without a public IP, just a private IP allowing only the private connectivity between the web tier and data tier and this one would be called **internal load balancer**. 

![image](https://github.com/user-attachments/assets/0ec55eef-ce9a-414e-ad80-c9ebf2628e8e)



### Summary

- Azure load balancer allows for even traffic distribution across Azure components and it supports both inbound and outbound scenarios. Both incoming and outgoing traffic. It is used by customers to provide highly available but also highly scalable applications. It supports both TCP and UDP applications. Supports both internal and external traffic with this public and internal load balancer.
- But Azure Load Balancer is not the only traffic distribution service in Azure

![image](https://github.com/user-attachments/assets/5d114cfd-6d57-4e92-b125-c0ce64938e80)



## Azure Application Gateway


![image](https://github.com/user-attachments/assets/3ea2afa3-d9e3-4897-a13a-3b0341d76be8)


If we are talking about traffic disctribution for resources, if that traffic is a web traffic (http traffic), you usually want to replace a load balancer with application gateway. This is because Application gateway is still a traffic distribution service but it is designed to support web traffic. So simply it has features that allow customers to better manage their web traffic.
Services like app services can also be used, so those services allow you to redirect traffic to any public IP or address. You are not limited to virtual machines when building scalable distributed applications. In case of building multi-tier application like previously, you would replace that public load balancer with application gateway

![image](https://github.com/user-attachments/assets/9464d73b-2bd7-4598-b5ae-7a1e1b7e2172)


### Summary
Application gateway is your web traffic load balancer in Azure with some features like web application firewall allowing you to scan for all the incoming traffic, redirection capabilities, session affinity when you want to be sure that your users are always directed to the same servers, URL routing, and SSL termination which allows customers to decrypt the traffic on the application gateway and send unencrypted version to the backend services to reduce the processing power required to decrypt every single request going to the backend. Increasing even more the scalability of your solution.

Just remember this is a load balancer that is designed to help you with distribution of web-based traffic

![image](https://github.com/user-attachments/assets/bc010b61-2489-45f5-8e8f-79e2dfd2e523)


## Content Delivery network (CDN)

CDN is one of those networking services that helps cutomers to build their applications. Let's take a web application as an example, every web application has some static content like Javascript files, style sheets, static pages or images. Normally, if developers don't know about the existence of services like content delivery network, what they will do is bundle this application and put it into app
