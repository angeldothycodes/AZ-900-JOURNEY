
![image](https://github.com/user-attachments/assets/4e1815ec-8d67-4709-9031-12724dbd3078)


# NETWORK SECURITY GROUPS

Let's say we have 4 servers. Two to handle web application traffic, on eserver to handle the business logic, and one more server to host our database. Depending on our architectural decisions, we can divide those into subnets. For example, have one subnet for all the microservices and web application traffic and another subnet to handle our data tier applications. Since those are subnets, they need to reside within a virtual network. If we create infrastructure like this, and we don't do anything else, all the traffic coming from the internet wil be allowed to all of these servers. Additionally, all the traffic between these servers will be allowed. Therefore, everything can communicate with everything. This is something we do not want to happen because our internet traffic should not be reaching our database and not all of these services should be able to communicate with each other.


![image](https://github.com/user-attachments/assets/bad86347-f13e-4953-abb7-076d9fdb4efa)


This is where **NETWORK SECURITY GROUPS** come in handly. For instance, place network security group on the first subnet allowing traffic from the internet to reach our web tier services. By creating Network Security Group on the second subnet, we can block the traffic coming from the internet but still allow the traffic coming from our own services


![image](https://github.com/user-attachments/assets/17d0f237-fc0f-4fee-b6e9-65968c24bc37)
