![image](https://github.com/user-attachments/assets/fa948d74-57a4-437f-adb6-241edd188f8e)


# Azure Key Vault

One of the most common scenarios that we see in Azure is building infrastructure: creating those virtual machines and disks.
Those disks will typically contain both operating system information but also your application data. All of our information on the disk needs to be encrypted so that if someone would get a hand of our disk they would not be able to decrypt the information and see what was on the drive. Typically, this is done by providing an encryption key. By default, Azure comes with a platform manage keys so all disks in Azure are encrypted by default but as customers, we can provide our own keys to encrypt but also decrypt virtual machine drives. Those are called **encryption keys**. Those keys can be stored using **Azure Key Vault**. The **Azure Key Vault** is our secure storage for disk encryption keys in
