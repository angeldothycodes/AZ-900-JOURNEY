
![image](https://github.com/user-attachments/assets/8675438d-735a-4f33-859f-ff18035131fa)

## Azure Advisor

 In order to talk about Azure Advisor, let's picture a scenario. Typically when building solutions in Azure, we will have multiple services. Services like SQL databases, web services, or virtual machines.Those services has to be set up by someone- our developers, administrators, operation teams, or just external vendors but the only problem with this approach is that none of us are experts when it comes to all of Azure services so it's very easy to miss some critical configuration that might impact your application or entire platform. Here comes Azure Advisor. It's a service that was created to continuously scan those services for all the improvements according to Microsoft best practices. 

Imagine: If you are starting with Azure, Microsoft might have some good tips for you that will improve how your application works and how you operate your entire Azure platform. The recommendations you can get are around cost of your Azure resources, their performance, reliability, security, and lastly, operational excellence.
All of the recommendations are then provided to either admins or developers. You can even setup some alerts to get automatically notified when there are new recommendations.


![image](https://github.com/user-attachments/assets/07917eda-58c3-4ca8-8b21-45702a0e6ead)


### Summary

- Azure Advisor is our personalized consultant service in Azure which is designed to provide us recommendations and best practives for:
   - **COST** to things like SKU sizes for our resources so we can downscale and save some money, idle services that can be deleted, or services where we can reserve the instances for longer periods to save a lot of money
   
   - Recommendations on **SECURITY**. Things like multi-factor authentication settings for our users
   
   - **RELIABILITY**. Previously, this was called High-availability but this now not only about keeping the application up and running but also protecting our data
   
   - We get recommendations about **PERFORMANCE**, again SKU sizes but in this case, should we scale up our application in order to get better performance, should we ugrade SDK versions if we are using the old one
   
   - Recommendations around **OPERATIONAL EXCELLENCE**. For example,  subscriptions limits that we're about to hit, any service health statuses that we should know about that might impact our application uptime.


- Azure advisor comes with **Actional recommendations**. As we have seen in the Azure portal, it is very easy to apply those recommendations directly from Azure advisor

- All of that is **FREE!**. If you are using Azure platform, if you use Azure services, you get all of those recommendations for free.



![image](https://github.com/user-attachments/assets/6eec0a3d-493e-4e62-aa3a-735d67b6c028)

