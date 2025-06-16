# Storage Services

![image](https://github.com/user-attachments/assets/ca902d0f-8544-411b-86c3-30f0ccf43b6a)


**Before we move to those services, let's talk about general classification of data**
- For **structured data**, the idea is very simple. This means your data is laid out so nicely that you can describe it using specific schema
- So for each table, each row of the table, you can define what are ht eproperties of each row, what are the type of those properties and each row that you insert into that table has to follow the schema.
- If you have multiple tables, you can define relationships between those tables. This is the scenario that you typically see in relational databases

- Second data is **Semi-structured**. In this case, you still have a table but each row within this table do not need to follow any specific schema. That means each row can have its own unique properties . The only common property is usually some sort of a key like an ID column.
- We can say this is a less fomalized way of storing our data.

- Lastly, we have **unstructured data**. Data like images, movies, applications of binary application files, txt file, and many more files. Files that do not follow structure that can represent pretty much any kind of data.


![Screenshot 2025-06-15 145902](https://github.com/user-attachments/assets/ffed9952-f55a-4860-91b9-0f0166cb2db6)



## Azure Blob Storage

We were talking about this unstructured data. Any kind of unstructured data can be called **BLOB**

**BLOB** stands for Binary Large Object. So any kind of files. You can put those blobs into Azure Blob Storage into something called container. Container is just a bucket for multiple blobs. You can have more than one container with an Azure Blob Storage. It is designed to allow both applications and users to work with unstructured files in the cloud.

![image](https://github.com/user-attachments/assets/7207b9c0-7f6f-4449-b4a2-f845d28915b4)


**Azure Blob Storage** is simply a service designed to store any kind of file in Azure. Remember that **blob is just a synonym for file** because Binary Large Object can represent anything. Additionally, there are three storage tiers. Storage tiers allow Microsoft to provide you better perfomance and better pricing depending on how often do you access your data. First tier is called **hot**, you use this for your frequently accessed data. If you're building web application and this web app is serving images to your customers then this would be the storage tier that you would use because hot storage tier provides the best performance for your files. 

But if your solution also store files that are accessed less frequently, then you can use **cool tier**. With **cool tier**, you are accepting lower availability and lower performance for accessing your files while maintaining high durability and getting significant discount for storing that data. This is the perfect solutions for storing older versions and backups for your applications.

If you have files that you never plan to access, like a long term backups. Let's say backup that you need to keep for 10 years, you can use **archive storage tier**. In this case, the availability is the lowest because retrieving that data might even take couple of hours but the price is also the lowest. You're getting 10x the discount for storing data in archived tier. This is the lowest price per gigabyte that you can get when storing data in Azure.

![image](https://github.com/user-attachments/assets/c14ebd3f-74c5-42cd-86fc-588c7f29fe56)


## Azure Queue Storage

- A small service but very significant when building applications.
- When you have application that have several tasks to be completed and each of those three tasks might take some time to complete - what you can do is output those into Azure queue as separate messages. This will allow background processes and other services to pick those messages from the queue at their own pace and let them process those asynchronously. This will not only offload your front-end application but also allow you to pick more suited services for the background processing.

![image](https://github.com/user-attachments/assets/9a5f20f5-0154-4094-8695-53bc4fb6e140)

**Azure Queue Storage** is a service that allows you to store small pieces of data - so called messages. So that you can build scalable asynchronous processing solutions in Azure.


![image](https://github.com/user-attachments/assets/34655ab6-c599-43ea-9e42-b7fba5553986)


## Azure Table Storage
  
This service was designed with semi-structured data in mind so that both users and application can output the semi-structured data form into tables. This table is part of table storage, you can have more than one table because table storage is just like a database where multiple tables are stored with your data. Just remember this is a semi-structured database. So there are no drawings, no schemas, just your data and a simple storage. This kind of databases are also called **noSQL** databases.

![image](https://github.com/user-attachments/assets/95f5592a-de03-4ef2-9900-d255980b8a7d)


### Summary
Azure Table storage is one of the storage services for your semi-structured data needs. You can work, insert update, and operate on the data in a semi-structured form. Take note, you use this kind of database when you don't need stuff like foreign joins, foreign keys, relationships, or when you don't need to follow any strict schema. Additionally, this service is designed for fast access. If you will store petabytes of data, you would still get your data within milliseconds if you would use compound key to access that specific rows. It is quite scalable even though it's a simple service. Similarly to blob storage, Microsoft provides many programming interfaces and many SDKs so it's very easy for your developers to use table storage when building solutions in Azure.

![image](https://github.com/user-attachments/assets/96fe81f6-cea5-40cf-a548-d7deee74ff8e)


## Azure File Storage
This service is similar to BLOB storage. As we said, BLOB is synonym for file. In this case, what's the difference between BLOB storage and file storage? let's start with semantic differences. First, in file storage, instead of blobs, you store files. Instead of containers, you have shares. And instead of blob storage, you have file storage. Semantically, they're pretty much identical, they work almost identical. The only difference is the way you acess them. In case of file storage, you access your shares via SMB protocol. This is a simple file share service, you might remember file shares when you go to, for instance, your Windows PC > right-click on your desktop > select Map network drive > it will appear in your PC just like any other drive on your machine except it's a remote drive somewhere on some sort of servers. In this case, that's exactly what Azure File Storage is for.

### Summary
Azure File storage is a service that will allow you access files via shared drive protocols. Whether you will use Windows or Linux machines, you can take advantage of file storage service. There are two common scenarios that this service was designed for. First one is extension of the on-premise file shares. If your company already has file shares that are used internally and they just need to extend those file shares with more space, they can leverage file storage to do that.
Second very common use case is lift-and-shift. Lift-and-shift means that you already have existing applications and you don't want to redesign those applications to take advantage of blob storage but you still want to extend or move files to Azure. In this case, you use Azure file storage to mount it as a local drive, yoou point your application to the local drive, they use native functionalities but in the end, this share is in Azure. So Automatically your files are saved to Azure. This gives to ability to take advantage of Azure features without any need to read these in your existing applications

Pretty much the major difference between file storage:
- You use file storage if you need that shared drive protocol
- If not, you design your applications and use blob storage

![image](https://github.com/user-attachments/assets/00ea12de-264b-4ff3-8a6a-5863ae216ade)


## Azure Storage Account
All the services we tackled on this chapter: blob storage, table storage, queue storage, and file storage are part of the bigger service called **Azure Storage Account**

<img width="377" alt="image" src="https://github.com/user-attachments/assets/4822c6a7-4514-485b-bc52-eb0ac1dc63e3" />


**Azure Storage Account** is simply a storage of services including those four that we just learned right now.

They are designed to allow customers to store files, messages, and semi-structured data in Azure.. very easily, very effectively, and at high scale. That high scale is quite high, up to petabytes of data. It just not scales very high, it also has high durability - eleven 9s (99.99999999%). If you pick the lowest replication on Azure storage account which is locally redundant storage. By default, ths provides eleven 9s of durability. The chance that you will lose you data is significantly low.. almost impossible. If you want, you can pick even better replication settings going up to 69s of durability and by default, this is the cheapest per gigabyte storage in Azure. And if you take advantage of Blob storage tiers, you can get very low price for very large amounts of data.


![image](https://github.com/user-attachments/assets/54cdb1fb-9e21-42f8-9330-5ce091b58056)


## Azure Disk Storage

![image](https://github.com/user-attachments/assets/01eaa057-c9c2-43f7-a3c0-ab2c01f85253)


It is used for virtual machines. When it comes to Windows VM, there are multiple partition- all those partitions are stored on one or more disks. In Azure, this is done via **disk storage service**. This storage service is simply set at disk emulation in the cloud, allowing customer to attach a persistent storage for virtual machines both for Operating Systems and application data.
Disks in Azure come with different sizes, different types so you can pick either SSD or HDD, and different performance tiers. Of course, the bigger and more performant the disk is, the higher the price. It is still good to have that choice because you can make the choice to grab this slower disk for your non-critical systems and development environments.
Disk storage allows customers to store their disk in unmanaged or managed form.
**Unmanaged** means each disk is stored as a file on a blob storage. It's called unmanaged because it is not managed by cloud provider. Customers are responsible for managing those blobs and those drives and the storage accounts. 
You can also use more popular option which is managed disks that means Microsoft is managing all the blob storage, all the files, and all the services behind the scene. Giving you a separate resource called manage disk which not only hides the complexity of managing the disk themselves but gives you some additional features which is very nice to have

![image](https://github.com/user-attachments/assets/a30c7447-404f-4da9-ba7e-639381fb5e24)

### Summary

**Azure storage account** is highly scalable and highly durable group of services for unstructured and semi-structured management. 
If you need general purpose file storage that fits pretty much any scenario in Azure, you can use **Azure blob storage**. 
If you need to take advantage of file shares in the cloud for lift-and-shift scenarios or extension of your on-premise file shares, you can use **Azure File Storage**. Additionally, if you're building scalable asynchronous processing architectures you can use **Azure queue storage** to deliver a service for very small messages and process offloading. 
If you need to have a small simple yet sclabale NoSQL database in Azure to store your semi-structured data then you can take advantage of **Azure table storage**
If you have virtual machines and you need to provide a persistent drive for those virtual machines, a simple disk emulation service in the cloud then you can take advantage of **Azure Disk Storage** 

![image](https://github.com/user-attachments/assets/a5799e6a-cb6b-4cc2-990c-644f935081c9)

