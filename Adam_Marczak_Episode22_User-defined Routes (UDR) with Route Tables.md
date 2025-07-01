![image](https://github.com/user-attachments/assets/282d0dce-eec3-4d20-aeed-fdd27ad595d3)

# User-defined Routes

**Routing** is a process of finding/selecting a path between two or more servers across one or multiple networks.

![image](https://github.com/user-attachments/assets/79e09694-905c-452d-8fe3-9e7dc04c328e)

In Azure, routing is set up by default. That means if we have 2 servers - one a web server and second an API server, both located in same virtual network in two separate subnets. If you would try to ping or connect from the web server to the API server, there would be a route setup for that already. If you also would connect to the internet from the web server, again the route is already setup as Azure by default creates an internal routing table and adds all the default routes in that table so that machines when provisioned can already connect to each other into internet with no issues at all. 

![image](https://github.com/user-attachments/assets/cd19cb40-3ce6-4d60-9dd2-f1973a68f863)


But if you want to change that beahvior, this is where **USER-DEFINED
ROUTES** come in play. Let's say we have a 3rd server called NVA for Network Virtual Appliance. This is simply a specific optimized virtual machine
