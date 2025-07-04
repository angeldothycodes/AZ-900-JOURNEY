![image](https://github.com/user-attachments/assets/6635aa7f-4ad5-4736-9412-0766c2472793)

This epsiode will talk about how Azure manages access to your resources with something called **Role-Based Access Control (RBAC)**

In previous episode, we've talked about how Azure Active Directory is a centralized service for identity and access management. That access management for Azure resources is done with role-based access control feature. 

To better understand how this works, let's start with what are roles. In Azure you have multiple resources like disks, virtual machines, SQL databases, or web applications, and many more. 

For all of those services, you can perform certain actions: create a disk, update that disk, maybe attach it to a virtual machine, start or stop this virtual machine, scale up your database, or just deploy web application. All those things that you can do in Azure with those services are so-called **actions**


![image](https://github.com/user-attachments/assets/8d1ea739-d7d7-415e-b812-a48464c441de)

**Action** as the name suggests defines what can be done with a certain type of service. Potentially, you could assign each specific action to users and applications to allow them to manage Azure resources. But it would be time consuming because there are literally hundres or even thousands of actions that can be performed in Azure. As such, it is easier to create a bundles of those actions so you can combine the actions that you are interested in like update disk, start and stop VM, and attach disk, and create a role called Virtual Machine operator. You can create as many rolse as you want for your organization. You can fine-grain your permissions for your applications and for your users however you need. All of those are **roles**. Azure comes with a lot of built-in roles, allowing you to manage your access to your resources and cover the most common scenarios very easily.
