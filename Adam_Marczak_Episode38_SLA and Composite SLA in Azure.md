<img width="942" height="419" alt="image" src="https://github.com/user-attachments/assets/f717f8f9-3608-499f-89a9-e39276e95e5a" />

# Service Level Agreement

**Service Level Agreement** is a formal agreement between service provider and a customer.


In case of Azure, this is between Microsoft and our company. So **SLA** in the context of Azure simply means a promise that Microsoft makes to us when it comes to the **service availability**. This is both uptime and the connectivity of that particular service.

**Availability** is a measure of time that this service remains operational.

<img width="770" height="380" alt="image" src="https://github.com/user-attachments/assets/96b99673-088f-4623-aefc-b4cdca9c4df6" />

If you search the web for Service Level Agreements in page, a page should come up whith the URL: **azure.microsoft.com**

<img width="790" height="335" alt="image" src="https://github.com/user-attachments/assets/0b53dd73-bf00-4a3b-9c0e-9c5555ac8396" />

From that page, you can type on the search bar the service that you want to know the SLA and it will return a page where the SLAs are detailed. 
Example:
<img width="674" height="459" alt="image" src="https://github.com/user-attachments/assets/cde83226-5e26-4660-b884-fbfdd7c942cf" />


Therefore, **SLA** is simple a promise of availability calculated per month. Every service in Azure has its own SLA definition because every single service can have different configuration and different availability associated with it.
The availability for most Azure services range from 99% to 99.999% but remmeber, most of Azure free service tiers do not have any kind of **SLA** associated. 

If you're using Azure and you're purchasing free services, they do not have any kind of SLA. This also goes when you're using service that are currently in **preview**, they do not offer **SLA** either.

Lastly, if the **SLA** is broken, you will get the discount. The so-called **service credit**.

<img width="328" height="340" alt="image" src="https://github.com/user-attachments/assets/325e666c-875b-41ba-96cf-3ecf4595c069" />

<img width="790" height="514" alt="image" src="https://github.com/user-attachments/assets/19571da3-98d6-490e-a6a5-7bcae73f72a5" />


## Composite SLA

It's a combined SLA of all of your application components. Therefore if you use multiple Azure services, you need to combine their SLA to calculate the SLA for your entire application

<img width="579" height="208" alt="image" src="https://github.com/user-attachments/assets/f4fcf697-d98f-40a5-a40f-432ccea44bef" />
