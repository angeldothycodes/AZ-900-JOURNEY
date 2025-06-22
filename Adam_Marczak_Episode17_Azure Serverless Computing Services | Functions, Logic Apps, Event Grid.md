![image](https://github.com/user-attachments/assets/e61e93ae-dc61-481f-bbaf-272711376087)![image](https://github.com/user-attachments/assets/01747425-bf4e-4d7a-a50e-4d47f46cb91e)

Serverless computing is a way of hosting your application in the cloud while completely abstracting the infrastructure part. We are just deploying our applications or out of the box products available in Azure and let Microsoft scale up and out of infrastructure to match our demand

![image](https://github.com/user-attachments/assets/4b6eb7c2-81ca-424c-a09e-b9302baebfb1)


## Azure Functions

We'ev already talked about **Azure Functions** as part of the Compute episode. 
Reitetraion: while they are a compute resource, they're also a serverless compute resource



Azure Functions is a service that allows customers to build application using code. 
Small pieces of code and host those as web services. In which case, customers create small pieces of code, package them, and send them to the function app. From that point onward, that is the serverless part because Azure Function app will grab your code and deploy this across multiple servers and allow external services to communicate with your application. If necessary, scaling up and down depending on your need.

![image](https://github.com/user-attachments/assets/0f5a4160-6f97-422c-b0b1-5bba40c1e03a)

### Characteristics

- Azure functions is our serverless coding platform, so-called **Functions as a Service**, allowing us to build nanoservices architecture and event-based applications.

- It also allows for quick scaling up and scaling down, and highly scalable because in this case, you can go up to 200 servers if required.

- Lastly, this service supports most of the popular languages and frameworks that are used for building web services. It means no need to learn any new languages to start using Azure Functions.


## Azure Logic Apps

This service allows to build workflows using a visual interface. Those workflows can represent both business scenarios but also cross-application integrations so you can build a simple step-by-step workflows or you can do something more complex with conditions, you can do loops if yiu need to or you can do parallel runs. All of those scenarios are very easy to implement using Azure logic apps. Additionally, each flow can be triggered by, for instance web request, you can trigger your flows using emails. You can also trigger them based on Office 365 events or you can trigger them based on what is happening in your Azure subscriptions bu there's more. There's over 200 connectors available to you so you can trigger your workflows not only based on Microsoft technologies but also other clouds, pther Software as a Service applications like Salesforce, SAP, etc, etc

Additionally, all of those 200 connectors allow you to use them within the flow so you can send web requests if you need to maybe send emails or save some files to blob storage. Or maybe instead write data to SQL database


![image](https://github.com/user-attachments/assets/133c34e3-f956-443c-9a83-c149387aad7f)
in our example
### Characteristics

- Aure Logic Apps are serverless enterprise integration service. That mwans we as a customers, we just designed the flows and let Microsoft handle the provisioning and scaling on the underlying infrastructure.

- Additionally, logic apps come with over 200 connectors. In our example, we are able to connect to Azure Blob storage and the email service without writing a single line of code. This service is specifically designed for the orchestration of both business processes but also integration workloads for our applications, daya, systems, and services. It is a powerful no-code service that means you can build your applications without writing a sinle line of code
