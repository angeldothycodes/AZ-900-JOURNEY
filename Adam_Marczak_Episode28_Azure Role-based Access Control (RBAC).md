![image](https://github.com/user-attachments/assets/6635aa7f-4ad5-4736-9412-0766c2472793)

This epsiode will talk about how Azure manages access to your resources with something called **Role-Based Access Control (RBAC)**

In previous episode, we've talked about how Azure Active Directory is a centralized service for identity and access management. That access management for Azure resources is done with role-based access control feature. 

To better understand how this works, let's start with what are roles. In Azure you have multiple resources like disks, virtual machines, SQL databases, or web applications, and many more. 

For all of those services, you can perform certain actions: create a disk, update that disk, maybe attach it to a virtual machine, start or stop this virtual machine, scale up your database, or just deploy web application. All those things that you can do in Azure with those services are so-called **actions**


![image](https://github.com/user-attachments/assets/8d1ea739-d7d7-415e-b812-a48464c441de)

**Action** as the name suggests defines what can be done with a certain type of service. Potentially, you could assign each specific action to users and applications to allow them to manage Azure resources. But it would be time consuming because there are literally hundres or even thousands of actions that can be performed in Azure. As such, it is easier to create a bundles of those actions so you can combine the actions that you are interested in like update disk, start and stop VM, and attach disk, and create a role called Virtual Machine operator. You can create as many rolse as you want for your organization. You can fine-grain your permissions for your applications and for your users however you need. All of those are **roles**. Azure comes with a lot of built-in roles, allowing you to manage your access to your resources and cover the most common scenarios very easily.

![image](https://github.com/user-attachments/assets/9a463e65-9601-4b74-b8f7-352faa2de229)

A **role** in Azure, a so-called role definition is simply a collection of actions that can be assigned to user or application identity and it will define which actions can be performed by that specific identity. 

A **Role definition** answers the question: what can be done? Which actions can you perform on Azure Resources.
Which brings us to the second topic. We already said the role needs to be assigned to identity. 

In this case, identities are so-called **Security Prinicpal**- objects with an Azure Active Directory that represent users or applications. Those could be **users** or **groups of users**. You can also assign roles to **service principals**, application accounts in Azure or application accounts that are tied to a specific service called **manage identity**. **All those are called security principals** and they can be assigned a role.

![image](https://github.com/user-attachments/assets/5e168bb3-874e-41bd-96ed-2ff6e8cc1680)


Let's say we have user called Adam. We can assign roles to Adam, let's say we can assign him a Virtual machine and database operator role so that Adam can perform support and operation tasks effectively. You can combine as many roles as you need to fit your needs. It is a common practice in Azure to give multiple roles to users and groups so that you can find great permissions and only grant the least privilege required to perform certain actions for specific usrs. You can also assign to Tom, let's say, a web developer if he is developing web applications. Or assign it to a group, in this case, a DB operator will be assigned to support L1 group so that both Jess and Pete who are part of this group would get that role assigned. 

It is quite important to understand that assigning a role to a group will affect all that users within that group. 
Those are exactly the **Security Principals** that we've been talking about.

![image](https://github.com/user-attachments/assets/a3659bf0-b2ca-4799-ae8f-da269f7dc0f0)


A **Security Principals** is an Azure Object and identity that can be assigned a role and those identity objects can be users, groups, or applications.

In this case:
**security principle** assignment **answers the question who can do it**. 

A **Role** answers the question **what can be done?**

![Screenshot 2025-07-05 110554](https://github.com/user-attachments/assets/9adfa8d2-1dc4-4228-bd38-b6746611f121)


Additionally, a role needs to be assigned to a scope. Where exactly those actions can be taken. Azure is organized in a hierarchy and a top-level object in Azure is called Management Group which allows you to group multiple subscriptions or multiple management groups. A **Subscription** is a top-level billing object so most of us will have a subscription asset our top level resource in Azure when we purchase our Azure subscriptions. Under each subscription, you will have multiple resource groups and since resource groups are a logical container for resources, under them you will have your own resources. When you assign a role to a scope, you can assign it any level.
In this case, if you assign it on a top-level, on management group level, that role will be inherited by all the child resources. If you assign a role on a management group level, that role will be propagated acroos all of these subscriptions, all of the resource groups, and all of the resources within this management group
 
![image](https://github.com/user-attachments/assets/56da0de5-52aa-495e-9237-d20157c92818)


If you decide to assign it on subscription level, it will affect only resource groups and resources within that subscription.

![image](https://github.com/user-attachments/assets/8c7d326f-59d8-48c6-94b2-5c673adfda78)

If you assign it in a resource group-level, the same thing applies. 

![image](https://github.com/user-attachments/assets/79884d8f-37bf-4c0e-a1ad-7b56a3ef3fbf)


You can assign it on any level that you want, even down to a resource level. You can even give me an access to your specific virtual machine or specific database only. And all of those are called **Scopes**

![image](https://github.com/user-attachments/assets/367d217b-a625-4c24-95ea-15c9cecd7384)

**Scope** is simply one or more Azure resources that the access is applied to. In that case, **scope assignment** answers the question **where it can be done?**.

![image](https://github.com/user-attachments/assets/dfdb82a2-2702-4249-836e-5b234e9ee188)


Let's follow this with an example:

**What can be done?** 
If you assign an **owner role** that means everything can be done, all the actions within Azure can be taken.
By **Who can do it?**, in this case if you assign it to user that means Adam can do everything.
The last question is **Where it can be done?**. Let's say you assign it to a virtual machine resource called DEV-VM.
In this case, you can read it from the top to bottom. Every action, everything can be performed by Adam on the DEV-VM virtual machine.

These three things are combined into something called **role asignment**. A **role assignment** is simply a combination of role definition, security principle, and the scope.

![image](https://github.com/user-attachments/assets/8876aaf7-8806-4205-af69-a17c5f1677f8)


![image](https://github.com/user-attachments/assets/d05a8527-d508-4d29-9995-00123ff49423)
