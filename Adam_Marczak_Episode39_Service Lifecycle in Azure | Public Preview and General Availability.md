<img width="478" height="268" alt="image" src="https://github.com/user-attachments/assets/1830a75e-f198-4eee-924f-991eee0cacf3" />


# Service Lifecycle in Azure | Public Preview and General Availability

Service lifecycle in Azure defines a process of how every Azure service is released for public use.
Every Azure service has its own lifecycle. The process of building Azure service follows a typical development path. It starts with requirement gathering> followed by development > testing. When the service is ready for wider use, it's then released to the public.
The first release to the public is done by releasing a preview version of the service. At this stage, most of the service functionality is ready so customers can use it and test it. This stage is called **public preview**. Think of it like a beta for your service. 
**Public preview** is designed to allow customers to experiment with the service, provide feedback, and for Microsoft to incorporate that feedback to improve the service before the final release is made.

When the service is validated, it's then released to the public for the second time, this time as a production-ready service. This stage is known as a **general availability**, in short **GA**. When the service is in **general availability**, Microsoft will keep improving the service and bringing new features in. Those features might land directly in GA but often they will be marked as a public preview too.
It's entirely possible to use this service that has been GA'ed long time ago that has still certain features in public preview.
You always need to be aware if the service that you're using and the features are already available for a general use, for the production use. From the perspective of the general public, these three stages is all that matters but it should be noted that Microsoft also has internal versions of the service before it's released to the public preview.
One of these stages is called **private preview**. It's released to a narrower audience. This stage is covered by an **NDA** and typically only high-profile customers who needed this particular feature. Microsoft, MVPs, and regional directors have access to this. This stage allows to prove the value and test the service before releasing it to a wider audience.

<img width="693" height="410" alt="image" src="https://github.com/user-attachments/assets/a334098e-57d2-491a-a3f3-9fab6edbd355" />

Certain things we need to note when it comes to public preview. Because public preview is this beta service so it has certain limitations and key things that you need to remember. First of all, if not very often, if not always, public preview services are out of SLA so using them for production workloads is not recommended.
Additionally, some services in preview are not covered by customer support.

<img width="609" height="440" alt="image" src="https://github.com/user-attachments/assets/42e1d029-2598-465e-a795-8e2eab2c1c0d" />
