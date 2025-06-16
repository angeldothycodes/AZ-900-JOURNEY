![image](https://github.com/user-attachments/assets/b036aa29-afea-4e4d-a783-a528d3e576d0)

In this episode, we will focus on **structured data** and **semi-structured data**.


## Azure Cosmos DB

In the last episode, we talked about how semi-structured data sets can be uploaded by either users or applications to a table entities hosted by Azure table storage service. In that sense, table storage and cosmos DB are very similar. Except for the table entities, you have collections. Instead of table storage, you have cosmos db.

![image](https://github.com/user-attachments/assets/286d0da0-c4e5-49cc-97c6-74a8b877d81b)


One of the primary features of cosmos DB is ability to replicate geographically. This is because Azure cosmos DB is available in many regions and data replication across thsoe regions is as simple as selecting checkboxes. Once that checkbox is selected, your data will automatically get replicated across Azure regions of your choosing. One of the cool features o cosmos DB is ability to not only read globally but also write globally. You can write to the closest data center available to your application and to your users. Besides its geo-replication capability, this database is also low latency database that means if you are operating on a small objects, it will return responses under 10 milliseconds. If you are building real-time applications, this might be the best choice for you of all of the services available in Azure 

![image](https://github.com/user-attachments/assets/70a206fb-7829-400f-ae79-029ec9f63bf4)


### Summary
Azure cosmos db is globally distributed noSQl database service in Azure allowing you to store your semi-structured datasets. Because semi-structured datasets do not require to follow schema, this is a schema-less database. It has ability to use one of multiple available APIs. Standard one is Core SQL API which allows you to query your data quite effectively. But if you're building applications based on MongoDB, cassandra, gremlin, table storage, you can very easily migrate to cosmos DB and use those respective APIs. Note that gremlin is for graph databases, so azure cosmos DB is not only a document database to store JSON files, you can also store graph data. Table storage API allows you to easily migrate from table storage to cosmos DB if you need that geo distribution or better performance. This database is was really designed to build either highly responsive or multi-regional applications or both.

![image](https://github.com/user-attachments/assets/ee4683f7-b3fa-4da3-8351-e1bb48905953)


## Azure SQL Database

This is our first service for storing strcutured data sets in Azure. This service allows both users and applications upload data to SQL database. With an SQL database, you define tables. Each table entity will have a specific schema that each row within that table will have to follow. Within the database, you can have more than one table with its own schema. Once the tables are defined, you can also define relationship to represent the business relationship between entities.

![image](https://github.com/user-attachments/assets/dcd5c267-a53c-4bdf-890e-ff01b64657a6)


Azure database is a relational database service in the cloud, this is a **Platform as a Service** but sometimes also called a **Database as a Service**. It is also a structured data service because customers are using schemas and relationships to model their data to represent their business. Working with structured data has its benefits. One of those benefits is SQL query language because databases like Azure SQL provides you with a rich query capabilities allowing you, your customers, you data engineers, data analysts to explore data in prtty much any way. They can join multiple tables, they can review all the data and return and extract the data and provide reporting capabilities for your organization. But Azure SQL is not only the database itself, it's a platform and as a platform, it provides customers with high performance, reliable, fully managed and secure database service. In this way, customers can focus on building applications and easily maintain security backups and monitoring for their SQL databases.

![image](https://github.com/user-attachments/assets/f3fba66e-45b2-4950-8f93-b4b641e4c650)


If you're working in the past with Microsoft BI technologies like SQL server, you might already know the products available in SQL server family like database, reporting services, integration services, and analysis services. If you move to Azure, those products are represented as separate services. From the SQL server family, only Azure SQL database is a representation of SQL server database and when it comes to other services, they were either migrated as a similar service or recreated with a new design in mind.

![image](https://github.com/user-attachments/assets/e6d5843f-4882-45bb-a857-c8c3fc3bc0aa)


## Azure SQL

It's a family of products with a similar capabilities. The one that we learned just now is **SQL database** which is based on a recent version, the most recent stable version of SQL server with a little bit less features designed for platform as a service offering. If you need full capabilities of SQL service from on-premise but in the cloud then Azure SQL also offers **managed instance**, this is much more pricey option but it gives you full capabiltiies. So if there are some features missing in SQL database, you can ue managed instance. There is also something called **SQL data warehouse**. This is a version of the SQL server for massively processing operations, pretty much for big data, data warehousing. Additionally, Azure SQL gives you an ability to install SQL server on a VM (**SQL VM**)- this will be an Infrastructure as a Service option but also very close to Platform as a Service because you get all the cool features of Azure SQL like backups, replication, security, monitoring, and automated updates on operating system but if you don;t like SQL server or you're migrating existing applications, you might like an option with different database engine. In Azure SQL, those options are **database for MySQL** and **database for PostgreSQL**. Those are open-source, very widely, very commonly used database engines on the market. If you're migrating existing applications, this might be the perfect option for you.

![image](https://github.com/user-attachments/assets/88542320-dc37-4b8c-988f-b689e583f887)


## Summary

The database services that we've learned today are **cosmos db** which is a globally distributed nosql database in the cloud allowing customers to take advantage of low latency, multi-master, which is perfect for building globally distributed applications and serverless applications.
We've also learned about **Azure SQL database** which is reliable relational database based on SQL sever. 
We've also learned about **Azure Database for MySQL** which takes advantage of Azure SQL platform offering with MySQL database engine. Similar case for **Postgre SQL**. Azure SQL delivers all the cool features but underneath, it runs on a postgreSQL database engine. Additionally, if you need a fully fledged SQL server, totally managed by Microsoft then you have an option with **Azure SQL managed instance**. This is more pricey option but with more features just like an on-premise SQL server.
If for some reason you need a total control over the infrastructure, then you can use **SQL server on a VM** which is fully fledged SQL server on infrastructure as a service.
Lastly, if you're working with big data, you might be interested with **SQL data warehouse**- part of Azure Synapse Analytics which is Massively Power Processing version of the SQL server called Big Data and Big Data Warehousing

![image](https://github.com/user-attachments/assets/73847ee2-1a85-4f14-8cdc-45c8e10ab660)
