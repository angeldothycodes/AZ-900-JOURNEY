![image](https://github.com/user-attachments/assets/ba6c191c-8d9e-4e8e-aafa-e1e22bb1fd08)

Because **Firewall** is a network security service that allows customers to monitor and control both incoming and outgoing traffic.

![image](https://github.com/user-attachments/assets/4113c0b2-019a-4744-b7ab-375991e36178)

There are many types of firewalls in the market from simple ones which allow you to filter traffic based on IP and protocol just like Network Security Groups (NSGs) or there are more advanced ones which allow you to filter traffic based on FQDN which is the domain name of the services or maybe inspect the body of the request itself to prevent from any kind of unwanted traffic.

In this episde, we will talk about service from Azure to provide us with that functionality called **Azure Firewall**.

# Azure Firewall

![image](https://github.com/user-attachments/assets/50ef6337-68b8-4d71-9079-af8ec7a6214c)


From the last episode, we had a scenario where we had three servers and we used route tables to route the traffic from our web servers to our virtual appliance which had a firewall installed but the problem with this design is that we had to manage all of that infrastructure and the firewall configuration from within that virutal machine. 

Instead of this, we can employ Azure service called **Azure Firewall**. A managed service from Azure which allows us to focus on the network configuration rather than management of the infrastructure but also centralization of our network configuration across multiple subnets and virutal networks and then we can decide based on our rules which traffic should go through and which one should be blocked.

![image](https://github.com/user-attachments/assets/103f504b-9a2f-4eb1-a79e-8b37f024714b)


![image](https://github.com/user-attachments/assets/e2c9f7e4-4c55-4099-a079-141b0e2e7067)
