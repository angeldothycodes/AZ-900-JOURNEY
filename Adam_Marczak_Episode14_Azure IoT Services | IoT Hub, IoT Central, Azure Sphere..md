![image](https://github.com/user-attachments/assets/ca77fb38-52ed-4af6-b8be-954a6ab83eaa)

### Internet of Things

What is **Internet of Things**? It is a network of internet connected devices, so called IoT devices. Those devices are embedded with everyday objects and they enable those objects to send and receive data from the cloud such as settings or telemetry. Most of us have some sort of IoT device at home whether it's as simple as smart lighting, a mobile phone, a plant wantering system, or something more complex like a door lock or a smart car. To build solutions in those IoT devices, you need a specific set of services for that purpose.


## Azure IoT Hub

Azure IoT hub allows for bi-directional communication between the cloud and IoT devices and then allows developers to take advantage of this information to provide insights monitoring and develop custom solutions for their IoT platform.

![image](https://github.com/user-attachments/assets/0d22b2a0-b444-4dd0-b329-306cf137c605)

The key things to remember about Iot Hubs are:
- It's a managed service for bi-directional communication between the cloud and IoT devices

- It's a Platform as a Service offering in Azure for IoT development

- It's highly secure, scalable, and reliable service for IoT

- IoT hubs perfectly integrates with a lot of Azure services and has a lot of SDKs for the most popular languages on the market so that your teams do not need to learn any new language to take advantage of IoT hub for their development purposes

- It also has support for multiple common standards on the market when it comes to communication protocols.


Just by looking at this list, we can very easily see that Microsoft created IoT hub to help developers build custom IoT solutions.

![image](https://github.com/user-attachments/assets/16144ea1-0a12-4b57-9880-4bcc81d221e4)


## Azure IoT Central

If building solutions from scratch is not something that your organization wants to do then you should look at Azure IoT central.
IoT central is very similar to IoT hub but it works on an entirely different level. It still allows for connectivity of your IoT devices with the cloud but **IoT central** as a service provides you a set of template for building applications using a standardized templates. It's an application delivery platform for IoT, for device management, and centralization purposes. This is an amazing solutions for organizations that want to take advantage of IoT and they don't want to build applications from scratch. 

![image](https://github.com/user-attachments/assets/7d945d82-e7ce-4d21-b2be-bc27af102541)


The key things that you need to know about IoT central is that this is an IoT application platform. It's a software as a service solution that allows you to use industry specific app templates to get out of the box solutions for your IoT devices and manage them at scale in the cloud. Microsoft with the service wants to allow their customers to build IoT solutions without the need to have very deep technical knowledge about IoT solutions. So the main goal of this service is to provide with application templates so you can very easily connect, manage, and monitor your IoT devices at scale.
Similarly to IoT hub, this service is highly secure, scalable, and very reliable so you can build you applications without worrying about the platform itself.
Lastly, this service is actully built on top of **IoT hub** and 30 other azure services.

![image](https://github.com/user-attachments/assets/9934615c-d2a9-4deb-b311-e34097b12d83)



## Azure Sphere

Azure Sphere is not really a service alone. It's a set of components allowing you to build secure IoT applications.
Let's say we have washing machines and we're building applications that will run on those washing machines. First thing that Azure Sphere delivers are Azure Sphere Microcontroller units. Simply said, those are simple chips that are built according to Microsoft standards and specifications. Microsoft then delivers this specification to hardware vendors so that they can build their chipsets according to the specification. Additionally, Azure sphere delivers an operating system. Microsoft manages this operating system to make sure that it's always upto date and that this system has the latest security patches applied on top of that. Third thing that Azure Sphere delivers is so-called **Azure Sphere Security Service**, this service is used for a secure communication between the cloud and the devices themselves so that your support team can apply updates to your application through that service but also Microsoft can apply updates to the operating system again through Azure Sphere Security Service. All of that is done to achieve one thing: to build secure end-to-end IoT solutions by creating a standardized certified chips, by creating secure operating system, and providing secure channel to communicate between devices in the cloud.

**Azure Sphere** is something bigger than just a service. It's set of tools for secure IoT solutions.


![image](https://github.com/user-attachments/assets/2d09f0f5-eb37-4095-ad60-ca31c9f4018d)


## Summary

- IoT hub is a managed service for bi-directional communication of IoT devices in the cloud. It's a platform as a service used to build custom IoT applications but your organization can also leverage existing industry standard-specific templates for building IoT solutions. In that case, they can use **IoT central** which is an IoT application platform with dozens of functionalities for provisioning management and monitoring of IoT solutions. Lastly, we have learned about **Azure Sphere** which is our end-to-end approach for building secure IoT solutions by providing both hardware operating system and communciation channels for securing our IoT solutions

![image](https://github.com/user-attachments/assets/1cf7ac50-fb31-495e-9ef7-f765a0109528)


