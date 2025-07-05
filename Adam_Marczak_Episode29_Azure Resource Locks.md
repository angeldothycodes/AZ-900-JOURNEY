![image](https://github.com/user-attachments/assets/c78c82c2-ea23-458a-9a07-a76496aa49b6)

# Azure Resource Lock

![image](https://github.com/user-attachments/assets/96640e12-280a-4935-bf68-c2a8468dfa17)


If you are a user of your Azure subscription and you have your Azure resources, when you are granted a role- let's say and owner, you can perform any action on this virtual machine like reading, creating resources, updating the virtual machine, or even deleting it.

The general issue with this is that owner can do everything including the deletion part. So if owner makes a mistake and deletes the virtual machine by mistake, it's gone. Microsoft won't be able to recover it. What you can do to prevent that is either take away owner privileges from that user or better, **apply a Resource Lock**.
When you apply a **Resource Lock** of type delete of this specific resource all of the actions will still be allowed base on the permissions, in this case Owner except for Delete. So even if the user is an owner of the resource, you won't be able to delete the resource if the **Resource Lock type Delete** is applied. If the user would need to delete the virtual machine, he would need to first remove the resource lock type delete but in Azure besides the Resource Lock that prevents you from deleting resources, there is one more Resource Lock type. 

If you have the same scenario, let's say this time Azure SQL, you can apply resource lock of type Read-Only. This resource lock works in an opposite way to how delete lock works. In this case, read-only lock will only allow you to read information about Azure resources and prevent you from running any actions that modifies this state of this Azure SQL. This is how you can prevent accidental changes and accidental deletion of your Azure resources while maintaining the privileges that you assign to your users. Maintain all the roles and only apply the locks whenever needed.
One thing to notice that you can manage the locks on individual resources-level, to better manage this on a resource-group level. 

Instead of creating locks on a specific resources, you can create a resource lock on a resource-group level. When you do it, when you apply a resource lock of type delete all of the resources within that resource group will be affected in the same way.

![image](https://github.com/user-attachments/assets/e46d1a52-d064-452a-9ea8-e30bcde9bcbb)

In this case, resource lock of type delete will prevent deletion of any resource within this resource group.

In Azure, the normal hierarchy goes from **Management Group > Subscription > Resource Group > Resources/ Individual Resources**

![image](https://github.com/user-attachments/assets/892828dd-adeb-424a-9a76-14047a17e695)

The highest level that you can apply lock to is at subscription level. In this case, the lock will affect all of the resource group and the resoruces within that specific subscription. You can apply resource lock on a resource group level or on the individual resources.

One of the most common use cases for using locks is locking the production services which contain your data. Because if you delete a storage account, Microsoft won't be able to recover that. All of the data that you store on the storage account will be lost.

![image](https://github.com/user-attachments/assets/d9909e36-d2fa-4072-a3f4-9583cf6cc60e)

