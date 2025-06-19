![image](https://github.com/user-attachments/assets/bbdb7188-9747-43c6-9c2c-7829759e0491)


**WHAT IS CONSIDERED BIG DATA?**
Big data is a field of technology that helps us with solving typical challenges around extraction, proecssing, and analysis of our data sets but in order to call something big data, certain characteristics has to be met. The first one is **velocity**. 

- **Velocity** means how fast is our data arriving. How fast, how often do we need to process that data. Are we processing that data in batches or maybe in real time?

- Second characteristic is **Volume**. We are talking about megabytes, gigabytes, terabytes, even petabytes of data.

- Thirs is **variety**. **Variety** means that how structured is our data. We are talking about tables or databases or something complex like video or social media information.

Based on these three characteristics, we can define whether this data is considered to be big data or not but as soon as we go high on one of those characteristics, traditional softwares will not be able to process this kind of data sets. 

![image](https://github.com/user-attachments/assets/dd425727-cdd2-4700-9225-1b6053f33fd9)


This is how big data technologies came to be. They were specifically designed softwares to help us with those kind of challenges which brings us to our first service: **Azure Synapse Analytics**

## Azure Synapse Analytics

In order to talk about Synapse Analytics and its benefits, we need to talk about how typical process looks like when it comes to transforming an analysis of our data. Most data engineers will start their process by identifying where is their data. Whether those are flat files, some web services, or databases and from there, a typical development process starts. Developers will first need to **ingest** their data from their sources to the cloud. Then they will need to **transform** those data sets and **store** them somewhere. After storing the data, expose this to other tools like reporting tools so that business users can take insights out of their data and make good business decisions. 
**Azure Synapse Analytics** helps with all of those steps first if all by providing a feature called **Synapse Pipelines**, this tool helps developers to ingest and transform their data using visual workflows. Additionally, Synapse Analytics comes with embedded **Apache Spark**, a leading technology for big data analytics and transformation. Also, their Synapse SQL are massively parallel processing database clusters based on a popular SQL server. This feature helps with transformation using typical SQL queries, storing of your data but also serving it to your reporting clients and all of that is baked into something called **Synapse Studio** which is a unified experience to manage all of those tools and features and perform all of your data transformation in a single place- all of that is nicely integrated with another Azure service called **Data Lake** so that ingrestion, transformation, and storage of our data can also be done directly on the data lake.


![image](https://github.com/user-attachments/assets/3b946f40-510f-43fd-b79a-a964c84126f8)



### Summary

**Azure Synapse Analytics** first of all is big data analytics platform. It's a Platform as a Service (PaaS) offering in Azure. Allowing users data engineers, data scientists to perform data analysis and data transformation over very large data sets and it has mutiple tools baked in. Tool like **Apache Spark** for efficient big data transformations.
**Synapse SQL** which allows us to use SQL server familiar tools with massively power processing design with dedicated or ad-hoc capacity
We also have **Synapse Pipelines** which allow you to visually build your ingestion and data transformation workflows 
All of that is combined into a single **Studio** experience, a unified experience for your data transformation needs.

![image](https://github.com/user-attachments/assets/d7950359-4208-45bb-8317-60f5c3cfbfe7)

## Azure HDInsight

