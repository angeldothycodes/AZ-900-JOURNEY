![image](https://github.com/user-attachments/assets/7ca6300b-32c6-41d4-82cc-fd8d93da52f4)


Before we move with DDoS Protection service, let's talk about what DoS stands for.

**DoS** means **Denial of Service**. It's a type of cyberattack where someone attacks your server that is exposed to a public internet with an intent to disrupt that service from working properly. This cause temporary or indefinite disruption of your service so users will not be able to use your services.

![image](https://github.com/user-attachments/assets/2475b925-541c-449c-a58f-b9f22879f4ed)


There are many types of Denial of Service attacks but most of them want to achieve the same thing: stop your service from working.
In general, Denial of Service attacks are pretty easy to prevent because you can just block the IP from which the traffic is originating. This is why most of the attackers instead of using one servers will employ multiple servers to attack your web services at the same time. This type of attack is called **Distributed Denial of Service**, so called **DDoS**

![image](https://github.com/user-attachments/assets/94d6ee4b-880b-473b-a0fd-9a104ac53634)



Preventing **DDoS** attacks is pretty tricky because not only you need to be able to identify which servers are attacking but also separate them from legitimate users trying to reach your servers and only filter the attacker out but still alow your users to connect.
This is where **Azure DDoS Protection** comes in

# Azure DDoS Protection

<img width="417" alt="image" src="https://github.com/user-attachments/assets/4dd1bd4a-57db-4631-bf22-5af4855421e2" />


If this scenario happened in Azure and our web server was hosted on one of Azure services, let's say Azure App Service, then in front of Azure App Service there would be a DDoS protection service which would filter the malicious traffic out and let the legitimate users in. One of the best things about DDoS protection is that the basic plan for DDoS protection comes with all of the Azure services by default. You don't even pay anything extra. It's already included in the price of that service but if you need more protection, this service comes with a standard plan which allows you to protect your application from some more sophisticated attacks. 

![image](https://github.com/user-attachments/assets/34f0189a-3407-42c4-8938-f28c5630b95e)
