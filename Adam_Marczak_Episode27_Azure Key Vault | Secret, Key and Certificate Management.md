![image](https://github.com/user-attachments/assets/fa948d74-57a4-437f-adb6-241edd188f8e)


# Azure Key Vault

![image](https://github.com/user-attachments/assets/f6027f0f-4d8d-4912-8b36-31831c9f80ff)

One of the most common scenarios that we see in Azure is building infrastructure: creating those virtual machines and disks.
Those disks will typically contain both operating system information but also your application data. All of our information on the disk needs to be encrypted so that if someone would get a hand of our disk they would not be able to decrypt the information and see what was on the drive. Typically, this is done by providing an encryption key. By default, Azure comes with a platform manage keys so all disks in Azure are encrypted by default but as customers, we can provide our own keys to encrypt but also decrypt virtual machine drives. Those are called **encryption keys**. Those keys can be stored using **Azure Key Vault**. The **Azure Key Vault** is our secure storage for disk encryption keys in Azure but it's not the only scenario that Azure Key Vault can help you with.

But it's not the only scenario that Azure Key Vault can help you with. For example, if you have a web application and you connect to your SQL database, those web applications will need to store connectivity information in their configuration like a server address, username and a password. This kind of information is typically called **application secrets** and Azure Key Vault can help us with storing and secure management of those secrets for our applications. There is plenty of additional SDKs so it's very easy to integrate your existing applications with Azure Key Vaults. A lot of Azure solutions also allow you to implement integration of key vault without writing a single line of code. 
Lastly, if your web applications are serving content to your users in a secure way over HTTPS, over encrypted channel through the internet, you can create a specific files called certificates. **Certificates** are complex objects for cryptography, they are used to encrypt traffic as it goes from your web servers to your users but certificates can also be used to provide a secure communciation and authentication channel across multiple services. 
Those two are just examples. In reality, there's plenty of other scenarios where certificates can be used and if you need a secure storage for those certificates, again, you can use Azure Key Vault


![image](https://github.com/user-attachments/assets/7f4926c0-2d89-4be9-9447-bc67103f3f1b)

That's pretty much what Azure Key Vault is, it's a secure storage for your application keys, secrets, and certificates.


![image](https://github.com/user-attachments/assets/ebb176ef-de90-4c96-a512-737fd38de811)

