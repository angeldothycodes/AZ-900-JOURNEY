What is the most important things you need to learn when working with Azure are the core building blocks for management of Azure services. Those building blocks consist of resources, resource groups, and resource manager .

We will also cover what are the benefits of using those core components when building solutions in Azure.

## Resources

When users go to Azure, they purchase services like SQL database, maybe web application hosting or simply a VM but it doesn't matter which service they buy. In the end, all those services are represented as a generic object called resource. You can think resources like objects used to represent your services in Azure. They are basically your contracts representing also a service lifecycle. As soon as you purchase a service in Azure, you create a resource.
As soon as you're done with the service and you delete it, the resource is also deleted.

Azure uses resources to save all the configurations that you make for your service. Pretty much any configuration option that you have for your service is represented as a property on that resource.

![image](https://github.com/user-attachments/assets/11f5e7aa-e9e9-462a-ae96-940f4a27ba7f)


All resources in Azure can be represented as a JSON template. There are four common properties across all resources: like **type**, **API version**, **name** and **location** and some other non-common properties taht are different and used to describe different resources, different services within Azure.

![image](https://github.com/user-attachments/assets/380850f6-e93c-492f-b444-1b1bd93602c6)


No resource in Azure can be created without something called **resource group**. A resource group is a logical container for only resources and it is requirement in order to create any resource in Azure. A resource group is a grouping of resources but you should use it to logically group related resources, it is not a hard requirement but research groups were created as a utility to manage Azure resources therefore you should take advantage of them. How do you know how to group resources together in resource group.

![image](https://github.com/user-attachments/assets/e2fba737-37e5-4508-8ba2-1ab469e1b23c)


There are many strategies to do so, for instance there could be a strategy that you would want to apply where you group your related resources by type. In that case, you could have resource group for your SQL databases and separate resource group for your web applications. More commonly used strategy is grouping resources by application lifecycle. Having your development resource groups spread from your production resource group so that you can apply different scripts, different policies, different security rules and different access management policies, you can also organize by departname name or use resource groups to group resurces for billing purposes. For instance, creating a separate resource group for each cost center within your organization. You can also create resource groups by location which is Azure region. That way it's easier for you to manage data sovereignty and security compliance requirements for your organization.


![image](https://github.com/user-attachments/assets/5212b610-ff75-45b8-bd80-f13d3bda87ed)



Take note that there's no one policy that will organize resources for every organization on the planet. As such, pretty much any organization uses a mix combination of those strategies like combining application names with environment names to give full separation of the application development life cycle with their production life cycle but also total separation across multiple applications - this is probably one of the most commonly used strategy on the market.

![image](https://github.com/user-attachments/assets/277260be-1b81-4279-ba01-82eb20993388)

