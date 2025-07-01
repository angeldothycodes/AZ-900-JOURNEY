
![image](https://github.com/user-attachments/assets/4e1815ec-8d67-4709-9031-12724dbd3078)


# NETWORK SECURITY GROUPS

Let's say we have 4 servers. Two to handle web application traffic, on eserver to handle the business logic, and one more server to host our database. Depending on our architectural decisions, we can divide those into subnets. For example, have one subnet for all the microservices and web application traffic and another subnet to handle our data tier applications. Since those are subnets, they need to reside within a virtual network. If we create infrastructure like this, and we don't do anything else, all the traffic coming from the internet wil be allowed to all of these servers. Additionally, all the traffic between these servers will be allowed. Therefore, everything can communicate with everything. This is something we do not want to happen because our internet traffic should not be reaching our database and not all of these services should be able to communicate with each other.


![image](https://github.com/user-attachments/assets/bad86347-f13e-4953-abb7-076d9fdb4efa)


This is where **NETWORK SECURITY GROUPS** come in handly. For instance, place network security group on the first subnet allowing traffic from the internet to reach our web tier services. By creating Network Security Group on the second subnet, we can block the traffic coming from the internet but still allow the traffic coming from our own services


![image](https://github.com/user-attachments/assets/17d0f237-fc0f-4fee-b6e9-65968c24bc37)



![image](https://github.com/user-attachments/assets/70289a22-ea81-4cda-805a-80e2b7eb924f)


# APPLICATION SECURITY GROUPS

Let's say our final configuration will allow the traffic going from the internet to our web services then block the traffic from the internet to our logic server so that only our web applications can connect to the services handling the business logic and then further this, only allowing the business logic web service to call the database servers and block the traffic from the web services directly to database. 


![image](https://github.com/user-attachments/assets/dcba768e-1588-4609-9157-d24a68357c42)


The internet traffic only reaches our web servers. Web servers will communciate with the business logic servers and business logic servers communicate with our database.


![image](https://github.com/user-attachments/assets/0fa481c7-28dd-42c0-ac3e-a882603391e0)

To achieve this using NEtwork Security Groups, we would need to use Static IPs of those machines in each single rule and manage this manually. This of course means a lot of maintenance effort. 


![image](https://github.com/user-attachments/assets/b95283ce-a72e-4a4c-9665-07cc1d296cf0)


You can solve this challenge by using **Application Security Groups**. Grouping your servers by their business purpose and then using those **Application Security Groups** instead of those static IPs in your network security rules.



![image](https://github.com/user-attachments/assets/6288ed2d-1ab9-4dd5-a7b1-174c3e77c225)

