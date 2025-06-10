What is the most important things you need to learn when working with Azure are the core building blocks for management of Azure services. Those building blocks consist of resources, resource groups, and resource manager .

We will also cover what are the benefits of using those core components when building solutions in Azure.

## Resources

When users go to Azure, they purchase services like SQL database, maybe web application hosting or simply a VM but it doesn't matter which service they buy. In the end, all those services are represented as a generic object called resource. You can think resources like objects used to represent your services in Azure. They are basically your contracts representing also a service lifecycle. As soon as you purchase a service in Azure, you create a resource.
As soon as you're done with the service and you delete it, the resource is also deleted.

Azure uses resources to save all the configurations that you make for your service. Pretty much any configuration option that you have for your service is represented as a property on that resource.

All resources in Azure can be represented as a JSON template. There are four common properties across all resources like type, API version, name and location and some other non-common properties taht are different and used to describe different resources, different services within Azure.

