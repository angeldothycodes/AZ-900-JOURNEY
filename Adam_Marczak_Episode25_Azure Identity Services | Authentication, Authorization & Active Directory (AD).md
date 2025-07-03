![image](https://github.com/user-attachments/assets/630fce6f-11f0-4e7c-8b29-5f45ff04c0c5)


## Identity

Identity in general means a fact of being something or someone. For example, our user accounts are considered **identity**. When we log into Azure portal, we use our own identities and we typically identify ourselves using username and passwords
but **identity** can also mean an application or server which will identify itself with a secret key or certificate.

![image](https://github.com/user-attachments/assets/aa414550-9cdc-4f2d-92f3-4b3558bc55a0)

The process of verification of that identity is called **authentication**. If user connects to your server, presented himself with username for instance Tom. Authentication server will require to present some authentication factor like a password, only then, Tom session will be established when identity is verified.
Whenever we logged into Azure portal, we needed to present our own credentials. This is the process of authentication.

![image](https://github.com/user-attachments/assets/1cfdbe61-1b2c-4724-8be9-3cc99184c83c)

Once identity is verified, there is another process called **authorization**.
When Tom will try to access one of our services, his account will need to be validated whether this account was granted an access by the resource owner. In this case, services can do it on its own or they can contact an external authorization server whether Tom has been granted access to this specific service.
This process of ensuring that only authenticated identities get access to the resources for which they have been granted access to by the resource owner is called **authorization**. We see that in every aspect of the management for the Azure platform. If we are able to go to Azure Resource Group that means we already have access to view that resource group. If we try to create or delete resource group or any service within that resource group that means we've been granted access to do so and this process of checking that is called authorization.


![image](https://github.com/user-attachments/assets/656d6e2c-54c0-43fe-8904-4be7aa70c24f)


Things like controlling, verifying, tracking, and managing access to authorized users and applications is called **access management**

![image](https://github.com/user-attachments/assets/018012e5-05f0-4a23-a85c-262c55024627)
