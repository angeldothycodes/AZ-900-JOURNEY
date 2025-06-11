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
Virtual machine scale set 
