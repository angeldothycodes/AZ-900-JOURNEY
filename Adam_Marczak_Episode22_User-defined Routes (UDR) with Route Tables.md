![image](https://github.com/user-attachments/assets/282d0dce-eec3-4d20-aeed-fdd27ad595d3)

# User-defined Routes

**Routing** is a process of finding/selecting a path between two or more servers across one or multiple networks.

![image](https://github.com/user-attachments/assets/79e09694-905c-452d-8fe3-9e7dc04c328e)

In Azure, routing is set up by default. That means if we have 2 servers - one a web server and second an API server, both located in same virtual network in two separate subnets. If you would try to ping or connect from the web server to the API server, there would be a route setup for that already. If you also would connect to the internet from the web server, again the route is already setup as Azure by default creates an internal routing table and adds all the default routes in that table so that machines when provisioned can already connect to each other into internet with no issues at all. 

![image](https://github.com/user-attachments/assets/cd19cb40-3ce6-4d60-9dd2-f1973a68f863)


But if you want to change that behavior, this is where **USER-DEFINED
ROUTES** come in play. Let's say we have a 3rd server called NVA for Network Virtual Appliance. This is simply a specific optimized virtual machine for certain tasks. In this case, this is a Virtual machine image that was created with a firewall inside. We can use this virtual machine to inspect all of the traffic before it will reach our internal servers. 

![image](https://github.com/user-attachments/assets/05baf416-32a9-44b8-b7c5-978a1fd545e0)


In this case, we can create something called a **route table**. 

![image](https://github.com/user-attachments/assets/e0ea4b3c-5b38-40b8-aea0-bdd3396b952b)



**Route Table** allows us to manage and override the default routes in Azure by creating our own routes. For example, by adding one route, we can affect how web server connects to API server by redirecting the traffic to the NVA which will inspect the traffic and forward or deny that traffic to the API server.

If you want, we can add one more route to affect the traffic going to the internet which will again go through the firewall if we want to.

![image](https://github.com/user-attachments/assets/79416e72-7422-402c-a2a7-1d55000559a1)




![image](https://github.com/user-attachments/assets/48ee5a48-b12b-430a-9d52-d5c48ebbefc1)


===============================================
===============================================
===============================================




![image](https://github.com/user-attachments/assets/dcb5ad37-2ccf-41df-9930-18fb7b0ab066)

![image](https://github.com/user-attachments/assets/5cf4b943-a1e8-44f5-9096-e14a3e60aa8c)



![image](https://github.com/user-attachments/assets/fc3d7e9d-8f47-4c27-b355-e0414d322811)



![image](https://github.com/user-attachments/assets/25c4ac55-0dde-42b0-ab5b-53d41dd16c81)


![image](https://github.com/user-attachments/assets/9ca65dee-2864-4f79-9c93-2e46236df3d2)



![image](https://github.com/user-attachments/assets/89432345-e160-4214-8977-46d806146f2b)


![image](https://github.com/user-attachments/assets/ac597f8a-a05f-42aa-a381-5ac1193b1929)



![image](https://github.com/user-attachments/assets/df7209cf-e05d-4be2-86af-5499b44d26e2)



![image](https://github.com/user-attachments/assets/b4912bb6-5725-498d-b1f6-041c63a4641a)



![image](https://github.com/user-attachments/assets/ffb1ab5e-3aad-4595-9d46-245ed861f606)
