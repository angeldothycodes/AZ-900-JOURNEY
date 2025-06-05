![image](https://github.com/user-attachments/assets/b55f2be0-d122-42b8-891e-326bffe662a6)



typical usage fluctuates over time and to match user demand, you want to allocate as many resources as you need at any given time. Ideally, you will only pay for those resources during the time of the usage and only as much as the resources that you consumed. The first thing you should note is that there is no upfront cost because with consumption-based model, you only start paying when you start using the resources and because cloud is elastic, you don't have to assign resources when you don't need them. This means no waster resources and you're not paying for them. Simply said, with consumption-based you only pay for the resources when you need them and you stop paying as soon as you don't need them 

![image](https://github.com/user-attachments/assets/630ef462-f573-477e-a72b-2cc9a3396f22)


In order for this model to work, we need to understand one moe thing. Let me use service like Virtual Machine as an example here. Charging for a service like Virtual Machine might be very tricky. What Microsoft did is created a few metrics that the price is based on. First, one is so-called **compute**. This is the power of the virtual machine, the size of the virtual machine that we purchased. If your usage changes per day, your size changes per day, you will be charged different amunt each day. Additionally, vitual machine usually there's a storage attached. You are priced for that storage separately so that if you have small machine but a lot of storage, you will pay different price that if you have big machine and very low amount of storage or some addiitonal metrics that are factored in, in the price of virtual machines like networking. Not reallythose factors is different per service because there are different services and they have different complexity because some services are easier to price. Other are harder but they are designed so that Microsoft can charge you appropriately to your usage. Therefore, in a consumption-based model, 
you have multiple pricing components per each service. Additionally, the charges are very granular if you only use virtual machine for 20 seconds, you will only pay for 20 seconds of usage. 

![image](https://github.com/user-attachments/assets/1e0741d3-2dd3-4341-bb50-9435f4f518a9)



As an example here, I want to quickly go to Azure portal which is a powerful web-based self-service portal allowing its users manage all the aspects of their other resources. Inside the Azure portal, there is one service that interests us right now is the **cost management service**. Inside that I can reveal the cost of my subscription. 

![image](https://github.com/user-attachments/assets/f4085bba-9d17-4189-944d-e0ef9cb5b57c)
