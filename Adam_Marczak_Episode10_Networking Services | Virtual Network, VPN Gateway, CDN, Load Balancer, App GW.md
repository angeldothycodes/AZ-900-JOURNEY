![image](https://github.com/user-attachments/assets/a646310f-fc0d-4f36-9b27-95801ffb7147)

![image](https://github.com/user-attachments/assets/78af2a61-8b30-44fa-b5c3-4bcfc1939e32)

## Azure Virtual Network

Imagine you have two resources in Azure, let's say 2 virtual machines. Because Virtual Machines are representation of the physical hardware in the cloud, they also need to be placed in the representation of the physical network infrastructure. That representation in Azure is called Azure Virtual Network. Virtual Networks allow their customers to create, manage, monitor, and secure connectivity between Azure resources but also between Azure resources and their on-premise environments. 

**Virutal Networks** can be segmented into smaller pieces called subnets. There are two main purposes for having subnets. One is to allow customers to manage their IP address allocation in a more efficient manner but also to group related resources together. So that you can apply filters and security rules across multiple resources within the same subnet.
For example, by grouping all the resources, hosting your web applications and only allowing web traffic to go to that subnet.
As a customer, you have a freedom of how you manage subnets and virtual networks. 
If you want, you can group multiple resources within the same subnet. It is you choice how you want to represent your networking infrastructure in the cloud.
There are many reasons why you would want to have virtual networks and many technical limitations forcing you to do that. For example, virtual network can ONLY reside within a single region and spawn resources from that specific region.
So if you will be building multi-region applications, you will end up with multiple virtual networks.
If you will want to connect multiple virtual networks you can
