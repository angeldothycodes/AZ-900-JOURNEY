![image](https://github.com/user-attachments/assets/a646310f-fc0d-4f36-9b27-95801ffb7147)

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
