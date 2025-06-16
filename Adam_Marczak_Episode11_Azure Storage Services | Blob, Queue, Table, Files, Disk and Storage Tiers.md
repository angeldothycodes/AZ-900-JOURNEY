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

![image](https://github.com/user-attachments/assets/00ea12de-264b-4ff3-8a6a-5863ae216ade)

