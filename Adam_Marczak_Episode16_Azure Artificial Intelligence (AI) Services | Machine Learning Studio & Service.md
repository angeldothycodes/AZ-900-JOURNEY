![image](https://github.com/user-attachments/assets/9bc5e8e3-4dfe-4df3-bc17-a7a70f11f816)


**AI** is a branch of computer science where we use our software to simulate human intelligence and capabilities

Whereas **Machine Learning** is a subcategory of AI where we use that software and teach it to draw some conclusions and make some predictions based on our data and the process of teaching the software to do that is caled building a model. 
The key service to do that in Azure is called **Azure Machine Learning**

![image](https://github.com/user-attachments/assets/f583ec29-9173-4144-888b-cf360e68da40)


## Azure Machine Learning

Typically, the process of building a machine learning model consists of training the model based on our data then packaging and validating that model. If we are happy with the results, we can deploy those models as a web services then monitoring those web services and retraining the model to get even better results. Azure Machine Learning is here to help us with this entire process by providing us with set of tools. Tools like notebooks written in Python or R or a visual designer which allows us to build machine learning models using a simple drag and drop experience directly in our browsers. Additionally machine learning models allows us to manage all the compute resources where we train, package, validate, and deploy those models so that we don't have to worry about Azure Infrastructure and underlying resources ourselves. Additionally, **Azure Machine Learning** comes with something called **AutoML**. This automated process allows us to drop random algorithms at our data and see which one scores the best and deploy that as our designated web service.
Lastly, there is also a feature of pipelines which allows us to build this entire process end-to-end whether we are using those notebooks, designer, or auto tools. This is complete end-to-end solution for building machine learning models.

![image](https://github.com/user-attachments/assets/c74c92c5-a05e-4759-8c84-44a8cecc8738)


### Summary

- **Azure Machine Learning Service** is an end-to-end cloud-based platform for creating, managing, and publishing of our machine learning models. This is a **Platform as a Service** offering in Azure. A top-level resource in Azure Machine Learning Service is called **Machine Learning Workspace**. Think of it like this: Workspace ties everything together. All the computer resources, all the permissions, all the runs, pipelines, experiments, history, connection to external services like Azure Storage Accounts, Container Registry, Deployments of your model. Literally everything is managed through Azure Machine Learning Workspace.
  
- **Machine Learning Studio** is the web portal that we were using for our end-to-end management of the workspace.

- Key features that you will get by using Azure Machine Learning Service are:
  - notebooks written in Python or R. Automated ML where you can throw a lot of algorithms and tweak some parameters to find the best algorithm and to build the best mode for your data. With Visual designer, you can build your machine learning pipelines without writing a single line of code. You can also manage your data and compute resources. So all the resources to manage and store your data as well as process those models and deploy them as a web services. Lastly, everything is nicely tied into other machine learning pipelines which allow you to orchestrate this model training, deployment and all the management tasks.

![image](https://github.com/user-attachments/assets/e3d0b557-e73b-4f2b-92cc-68ecaa2cfa7b)
