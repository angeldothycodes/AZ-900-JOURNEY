![image](https://github.com/user-attachments/assets/438f6b0f-c7e2-4396-a414-2e8f9187c9df)

Objective is to talk about what Azure policy is and what are the typical scenarios in which you would want to use Azure Policy in your own Azure environment. 

As we were progressing throughout all of our episodes, we've learned that we are a customers of Azure and as customers, we go to Azure portal to create Azure services. We do that by specifying the common properties for each service. We specify the type of the service that we want, let's say an App Service which can host our web applications, a location which is also called **Azure Region**, in this case German and other common properties for specific services, let's say SKU. When we choose all of those properties, we send a request to Azure. We do that through either Azure portal or we can do it through Azure PowerShell CLI or any other tool of our choosing. What Azure does first is validating this request. Azure will check whether the service is a proper service, did we fill all the required properties, is the combination of the properties correct, is this service available in this region and many other things. Once the request is validated, the next thing being checked is permissions. Azure will check whether the user that submitted the request to create this specific Azure resource has all the permission required to create the service and if it does, it creates the service with the properties that we specified.

![image](https://github.com/user-attachments/assets/92884012-dcf1-4eb9-beaa-9a00146a7d5f)

But there's one more thing that Azure does before creating that service which is checking for policies. **What is policy?**
**Azure Policy** allows you to check for Azure Resource properties and then make decisions based on the values of those properties.

![image](https://github.com/user-attachments/assets/16b92139-5750-4915-8c77-9cade1d6c331)

For example, let's say we have a company and our company has some data sovereignty requirements that needs to be met in order to create aplications. Let's say because of the security policy our data might never be processed outside of the German borders, to do that we need to ensure that all of our services that will be created in Azure will be in location Germany.

To do that we can create Azure Policy. We create a policy in which we'll check for certain other properties. In this case, location. Then we can create a rule and check whether location is Germany then we can allow for the deployment but if value is anything else then deny the deployment. This is called **Policy Definition**. In your Azure environment, you can create as many policy definitions as you want in order to match your internal standards.
