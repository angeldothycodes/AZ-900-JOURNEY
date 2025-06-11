![image](https://github.com/user-attachments/assets/348c0319-e789-4a36-a33f-6cc97f473c95)

> These services are part of so-called **compute services**
> **Compute Servics** is a category of services in Azure, allowing you to build and run cloud-based applications. Whenever this is a web application, web service, some scripting, desktop applications, compute services are here to help.
>
> ![image](https://github.com/user-attachments/assets/88a20e96-707d-4202-a80a-a424f05a8e0c)


 ##Virtualization
First service on the list is virtual machine but in order to talk about virtual machine, let's talk about virtualization in general.
If you have a physical server, physical machine, what you will do first is install operating system which will have standard components like file systems, some services, some ports, and other configs. If you will want to run applications on this physical machine, you will simply install them on that operating system. but the problem with hosting multiple applications on the same operating system is that they will share the same file system, same services, same ports, and other configs. Because there is no boundaries between those applications, at some point or another, they will collide and it doesn't matter whether they will use the same service or same ports at some point, they will collide which is not good.
The thing you can do to avoid that is to use **virtualization** where on the physical machine, you install operating system. But additionally, you install virtualization software, virtualization software will allow you to create virtual machines - an emulation of a physical machine. That machine since is an emulated physical machine, will still have to get its own operating system and on that operating system, you will be  able to host your application and this application now has its own sandbox - it doesn't matter what it will do on this operating system, it will not impact any other application because other applications will be hosted on separate virtual machines with their own environments. This gives you a full separation and allows you to virtualize, emulate multiple physical machines using a single physical machine.

![image](https://github.com/user-attachments/assets/06ca3515-1a85-43a9-89c2-75a09cad2936)


Simply said, **virtualization is emulation of physical machines**. It gives you ability to create a different virtual hardware config per machine and per application.

Additionally, you are able to install different operating system per machine per application. So if application needs different systems, this is a way to go and because those are totally separate machines, each application can freely use its own file system services, ports, install any middleware or apply any configuration it needs to run and vritualization in the cloud is done through **Azure virtual machine service**. The process is fairly simple. You either grab Microsoft-prepare virtual machine images- whenever this is Ubuntu, Windows, or a cold machine, Microsoft already prepared virtual machine images for you in the marketplace that you can start from or if you want, you can configure your own system, install services, runtimes, applications, and ask your developers to prepare an image- a custom image for your own company and put that image into some storage. 

An **Azure virtual machine service** grabs those images and allows you to choose a custom or marketplace image to start creating new virtual machines and exposing them to your users. Doesn't matter which one you choose, in just a couple of minutes a virtual machine will be provisioned and ready to use.

![image](https://github.com/user-attachments/assets/93de82ec-24f1-4cfc-a576-a8c914255e04)

**Virtual machines** are of course **Infrastructure as a Service**. That means you are responsible for managing both application, platform and operating system configurations because of that you have total control over the operating system and the software running on it and as such you have a support for marketplace but also customer-provided images so you can prepare your own images as a starting point for the virtual machines containing your organizational setup out of the box.


With that said, this service is best-suited for a custom software requiring system configuration or lift-and-shift scenarios. So moving your on-premise application to the cloud without a need to redesign. When it comes to supported scenarios, you can run pretty much any application, any scenario using virtual machines whether this is a web application, web service, maybe a database, desktop application, or using this as a jumpbox to connect to a secure environment or just data gateways, or many other scenarios that virtual machines can support.

![image](https://github.com/user-attachments/assets/e2401182-eac0-4373-a44c-684f2a32f8cf)


**To summarize**, virtual machines they give you a lot of control over the system but that also gives you additional maintenance therefore I rate them high when it comes to control and maintenance. They have no autoscaling feature threfore you always work with one node, one virtual machine at a time. As such the scalability of this solution is quite low because you can't autoscale. The only way of scaling is vertical scaling by adding faster CPUs or more memory, faster drives which brings me to the second point. 


##Azure Virtual machine Scale Sets
With this service you pink an image, whenever this is a custom image or a marketplace image.This image is automatically scaled across multiple virtual machines. Those virtual machines are hidden behind a load balancer which redirects the traffic from your users or applications to one of those virtual machines within the scale set. The amount of virtual machines can be set statically by saying 3,5, 10 or 100 or automatically with autoscaling feature. You can increase the amount of virtual machines in scale set or decrease the amount based on your application demand. 


In that case, virtual machine scale sets are still Infrastructure as a Service because you are still managing the virtual machines, you need to still prepare images, but they are set of identical virtual machines created from the same image. As such, they have built-in auto-scaling features allowing you to create and delete virtual machines based on demand and they are designed for manual or out-of-scope workloads - things like web services, batch processing, etc. This is your way to scale-out with virtual machines in the cloud.

![image](https://github.com/user-attachments/assets/064f2b55-4d97-404b-850f-b11fe28176b1)

In this case, you still have a quite of lot maintenance but high degree of control over the virtual machine scale sets but in this case, you are getting auto-scaling features so you can scale up to maximum of a thousand of 600 depending whenever this is custom or marketplace image which makes scale sets as one of the most scalable services in Azure. If you want to decrease the maintenance required, you can move away from virtual machines into containers.

![image](https://github.com/user-attachments/assets/ca1c53dc-5ebf-4770-a4e8-e7df13913098)


## Containers vs VMs
You can move away from virtual machines into containers. Containers are a little bit different than virtual machines. While there is still physical machine, there is still operating system unerneath. But instead of installing virtualization software, we install container runtime within container runtime, you install containers. **Container** is a sandbox environment for each application and you can have multiple containers within a single runtime. The major difference here is there is no operating system replicated across each container. As such, the footprint of the container is much smaller than the one of the virtual machine.

![image](https://github.com/user-attachments/assets/6f61dada-22c6-49f3-8fdf-e48a60c1a8ed)

##Containers
- Don't have their own operating system, they actually host operating system but because application needs operating system to run, they emulate it. So while virtual machines emaulate hardware, containers emulate operating system to provide the sandbox environment for your applications. Because of that they are more lightweight than virtual machines, therefore there's less development effort required for your team, there's less maintenance because you don't need to maintain the operating system patches, updates. Becaue there's no operating system, there's less compute than storage requirements from those containers, as such, you can respond quicker to demand so you can autoscale faster than with Virtual machines but at the same time, they are pretty close to virtual machines therefore they allow you to run pretty much any scenario in the cloud. That's why containers are so popular recently on the market.

![image](https://github.com/user-attachments/assets/b9ac4189-8305-434a-90c2-b0a854ef418c)


##Azure Container Instances (ACI)

Our first service for containers is called **container instances**.

![image](https://github.com/user-attachments/assets/72bbc253-a077-491c-9425-cd2f84911607)


When it comes to container instances, instead of bundling entire system, you just grab the application, grab the configuration, and other runtime, middleware, software that you need for this application to run, you ask your developers to bundle this application into a container image and host it into container repository.  **Container repository** is a simple storage service where you host your own images. Similarly to virtual machines, there are public marketplace and public repositories of other images for containers as well. You can then grab any of those images and push it to container instance which will create a container group a simple virtual machine underneath the scenes and host your containers. Some containers might be exposed to users, some might not. It depends on what container really does. If it's web application, it will be exposed to users. If it's a simple batch script, maybe it won't. You can create more container group and host small container depending on your needs.

**Summary**

- Container instances is your simplest and fastest way to run a container in Azure
- First service categorized as **Platform as a Service**
- Sometimes called Serverless containers because you can actually abstract from the managing of the servers underneath completely
- This service is designed for small and simple web applications running bakground jobs, maybe some scheduled scripts.

![image](https://github.com/user-attachments/assets/3bb0ca08-8fec-4bcb-8c2f-c735b82f3dd8)



When comparing container instances to virtual machines and scale sets, you still maintain some degree of control because you are virtualizing operating system so you can install run extra runtimes, extra software but it's still much less than maintaining full-fledged operational system. In case of container instances, there's no autoscaling but the cool thing is that at minimum, you don't need to run any servers so you can have zero nodes running, if you don't need any but at maximum, you can have 20 container groups therefore the scalability of this solution is not that great but it's nothing bad. This service is simple for simple use cases. If you need scalability, there are other services that deliver you that. Service like **Kubernetes Service**
