# Infrastructure as a Service (IaaS)

- **IaaS** is the most flexible cloud service model, giving you maximum control over your resources.
- The **cloud provider** manages:
    - Physical hardware
    - Network connectivity to the internet
    - Physical security
- **You** are responsible for:
    - OS installation, configuration, and maintenance
    - Network setup and management
    - Database and storage configuration
    - Patching, updates, and security

## Shared Responsibility Model

- In IaaS, most responsibilities are on you, except for physical infrastructure and connectivity, which the provider manages.

## Common Scenarios for IaaS

- **Lift-and-shift migration:** Move your on-premises workloads to cloud-based infrastructure with minimal changes.
- **Testing and development:** Rapidly create and replicate dev/test environments, start or stop resources as needed, and retain full control.

---

> **Key Benefit:**  
> IaaS lets you rent datacenter hardware in the cloud and gives you the freedom to configure and manage everything else.



# Platform as a Service (PaaS)

- **PaaS** is the middle ground between IaaS and SaaS.
- The **cloud provider** manages:
    - Physical infrastructure and security
    - Network connectivity
    - Operating systems, middleware, development tools, and business intelligence services
    - Licensing and patching for OS and databases

- **You** focus on:
    - Building and deploying applications
    - Customizing and managing your app code
    - Some network/app security and configurations (varies by setup)

## Shared Responsibility Model

- Responsibilities are split:
    - Provider: Hardware, OS, platform tools, patches, updates
    - You: Application logic, data, and sometimes network/app security

## Common Scenarios for PaaS

- **Development framework:** Rapidly develop or customize apps with built-in tools and frameworks (less coding needed, includes scalability and high availability).
- **Analytics/Business Intelligence:** Use built-in tools for data analysis, pattern recognition, and predictions to support business decisions.

---

> **Key Benefit:**  
> PaaS lets you develop, run, and manage applications without worrying about managing infrastructure, OS, or platform tools.

