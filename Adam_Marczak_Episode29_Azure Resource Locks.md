![image](https://github.com/user-attachments/assets/c78c82c2-ea23-458a-9a07-a76496aa49b6)

If you are a user of your Azure subscription and you have your Azure resources, when you are granted a role- let's say and owner, you can perform any action on this virtual machine like reading, creating resources, updating the virtual machine, or even deleting it.

The general issue with this is that owner can do everything including the deletion part. So if owner makes a mistake and deletes the virtual machine by mistake, it's gone. Microsoft won't be able to recover it. What you can do to prevent that is either take away owner privileges from that user or better, **apply a Resource Lock**.
When you apply a **Resource Lock** of type delete of this specific resource all of the actions will still be allowed base on the permissions, in this case Owner except for Delete. So even if the user is an owner of the resource, you won't be able to delete the resource if the **Resource Lock type Delete** is applied. If the user would need to delete the virtual machine, he would need to first remove the resource lock type delete
